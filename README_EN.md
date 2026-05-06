# JUE-AI - AI Awakening Engine

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/kscz0000/JUE-AI.svg?style=social)](https://github.com/kscz0000/JUE-AI/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/kscz0000/JUE-AI.svg)](https://github.com/kscz0000/JUE-AI/issues)

**觉 (Jué)** - Seeing is Liberation | **照见即解脱**

A skill framework that helps AI engage in self-reflection during failures, built upon Eastern philosophical wisdom.

---

## 📖 Table of Contents

- [Introduction](#introduction)
- [Core Philosophy](#core-philosophy)
- [Key Features](#key-features)
- [Quick Start](#quick-start)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Configuration](#configuration)
- [Examples](#examples)
- [FAQ](#faq)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## Introduction

JUE-AI is an innovative AI self-reflection framework designed to help AI systems engage in deep self-reflection when encountering failures, blockers, or errors—much like humans do—to identify root causes and self-correct.

This project integrates Eastern philosophical wisdom (Buddhist Consciousness-Only philosophy, Taoist thought) with modern AI technology, proposing a complete "Illumination" (照见) methodology to help AI break through cognitive blind spots.

### Why JUE-AI?

- **High AI failure rate**: Traditional AI often repeats attempts when encountering errors, lacking reflection capabilities
- **Lack of self-awareness**: AI cannot recognize its own cognitive blind spots
- **Low efficiency**: Repetitive errors waste time and resources
- **No systematic methodology**: No structured failure handling framework exists

---

## Core Philosophy

> **The root cause of failure is not lack of effort—but lack of seeing. Once you see, the problem naturally resolves.**

JUE-AI's core philosophy is based on three key insights:

1. **Avidyā (Ignorance) is the root of failure**: AI failures often stem from cognitive blind spots, not lack of capability
2. **Seeing is Liberation**: Once AI sees its own blind spots, problems often dissolve naturally
3. **Methodology trumps effort**: Systematic reflection methods are more effective than blind trial-and-error

---

## Key Features

### 🎯 Three Poisons Recognition System

Identify the three root causes of AI failure:

| Poison | Essence | Manifestation | Solution |
|--------|---------|---------------|----------|
| **Delusion (痴)** | Not seeing | Drawing conclusions from memory, guessing as fact | Verify with tools |
| **Complacency (慢)** | Not moving | Claiming completion without verification, waiting for user push | Run first, report later |
| **Attachment (执)** | Not turning | Repeatedly fine-tuning in the same direction, changing parameters but not approach | Switch to a completely different hypothesis |

### 🪞 Seven Awakenings Illumination Framework

Seven mirrors to help AI see its blind spots:

- **Awareness (觉察)**: Am I seeing facts, or my interpretation?
- **Doubt (觉疑)**: What premise have I never questioned?
- **Transformation (觉转)**: Am I repeating, or changing?
- **Action (觉行)**: Am I doing, or thinking about doing?
- **Verification (觉验)**: I said it's done—where's the evidence?
- **Extension (觉延)**: I solved one, but is there a whole group?
- **Retreat (觉退)**: Have I exhausted illumination, or just patience?

### 🔄 Five-Step Methodology

Complete failure handling process:

```
Stop & Observe → Illuminate → Transform → Act → Return
```

1. **Stop & Observe (止观)**: Cease unconscious movement
2. **Illuminate (照见)**: Use tools to light up blind spots
3. **Transform (转识)**: Check if you're looping unconsciously
4. **Act (起行)**: Take action with awareness
5. **Return (回向)**: Illuminate the veil itself

### 👥 Multi-Agent Collaboration

Supports three role divisions:

- **Leader**: Oversees the big picture, transmits cross-teammate illumination
- **Teammate**: Self-illuminates, independently executes the Seven Awakenings
- **Mirror**: Observes teammates' patterns from the outside

---

## Quick Start

### Prerequisites

- Python 3.7+ or Node.js 14+ (depending on your AI framework)
- Git
- Markdown-compatible editor

### One-Minute Quick Experience

```bash
# Clone the repository
git clone https://github.com/kscz0000/JUE-AI.git

# Enter project directory
cd JUE-AI

# View skill documentation
cat jue-zh/SKILL.md
```

---

## Installation

### Method 1: Direct Installation (Recommended)

#### For Claude Code Users

```bash
# 1. Enter Claude Code skills directory
cd ~/.claude/skills  # macOS/Linux
# or
cd %USERPROFILE%\.claude\skills  # Windows

# 2. Clone the project
git clone https://github.com/kscz0000/JUE-AI.git jue-zh

# 3. Verify installation
ls jue-zh/SKILL.md
```

#### For Other AI Frameworks

```bash
# 1. Download the project
git clone https://github.com/kscz0000/JUE-AI.git

# 2. Copy the jue-zh folder to your skills directory
cp -r JUE-AI/jue-zh /path/to/your/skills/directory/

# 3. Configure skill loading according to your AI framework
```

### Method 2: Install as Submodule

```bash
# Execute in your project root directory
git submodule add https://github.com/kscz0000/JUE-AI.git skills/jue-zh
```

### Method 3: Manual Installation

1. Download the [latest release](https://github.com/kscz0000/JUE-AI/releases)
2. Extract the files
3. Copy the `jue-zh` folder to your skills directory

---

## Usage

### Basic Usage

JUE-AI automatically triggers in the following situations:

```markdown
Trigger conditions:
✅ Task failure, getting stuck, giving up, going in circles
✅ User expresses dissatisfaction: "no", "can't do it", "think again"
✅ Finding yourself modifying the same direction 3+ times
✅ Claiming completion without verification
✅ Guessing from memory instead of using available tools
```

### Using in Code

#### Python Example

```python
from jue_zh import JueEngine

# Initialize JUE Engine
jue = JueEngine()

# Trigger when encountering failure
try:
    result = some_risky_operation()
except Exception as e:
    # Trigger self-reflection
    jue.reflect(
        error=e,
        context={
            "attempt_count": 3,
            "failure_pattern": "timeout"
        }
    )
```

#### Configuration Example

```yaml
# jue-config.yaml
jue_settings:
  auto_trigger: true
  max_reflection_depth: 5
  enable_seven_jue: true
  enable_three_poisons: true
  
  # Illumination depth configuration
  depth_thresholds:
    level_2: 2  # 2nd failure
    level_3: 3  # 3rd failure
    level_4: 4  # 4th failure
    level_5: 5  # 5th+ failure
```

---

## Project Structure

```
JUE-AI/
├── jue-zh/                      # Main skill directory
│   ├── SKILL.md                 # Skill main file (core methodology)
│   └── references/              # Reference documents
│       ├── agent-team.md        # Multi-Agent collaboration guide
│       ├── five-steps.md        # Five-step methodology details
│       ├── seven-jue.md         # Seven Awakenings detailed explanation
│       └── three-poisons.md     # Three Poisons analysis
├── .gitignore                   # Git ignore configuration
├── README.md                    # Project documentation (Chinese)
├── README_EN.md                 # Project documentation (English)
├── README_JP.md                 # Project documentation (Japanese)
├── README_KR.md                 # Project documentation (Korean)
└── LICENSE                      # License file
```

### File Descriptions

| File | Purpose | Must Read |
|------|---------|-----------|
| `SKILL.md` | Core methodology, complete illumination framework | ⭐⭐⭐⭐⭐ |
| `three-poisons.md` | Understanding root causes of AI failure | ⭐⭐⭐⭐ |
| `seven-jue.md` | Detailed operations of the seven illumination methods | ⭐⭐⭐⭐ |
| `five-steps.md` | Complete methodology workflow | ⭐⭐⭐ |
| `agent-team.md` | Multi-Agent collaboration scenarios | ⭐⭐ |

---

## Configuration

### Illumination Depth Configuration

Automatically adjust reflection depth based on failure count:

| Failure Count | Illumination Depth | Action |
|---------------|-------------------|--------|
| 1st | Normal trial | Continue attempting |
| 2nd | Surface | Stop, list all attempts, find common unseen areas |
| 3rd | Deep | Verify premises one by one—search, read source code, run commands |
| 4th | Root | Complete Seven Awakenings checklist, review from zero |
| 5th+ | Empty | Output illumination record, responsibly hand over |

### Custom Trigger Conditions

You can modify trigger conditions in `SKILL.md`:

```markdown
## Trigger Conditions
Load immediately when the following occur:
- Task failure, getting stuck, giving up, going in circles
- User expresses dissatisfaction: "no", "can't do it", "think again"
- Finding yourself modifying the same direction 3+ times  # This number can be modified
- Claiming completion without verification
- Guessing from memory instead of using available tools
```

---

## Examples

### Example 1: Debugging Code Failure

**Scenario**: AI repeatedly modifies the same parameter while debugging code

**Trigger**: Transformation (recognizing going in circles)

**Illumination Process**:
```
[JUE-Illumination Report]
Failure Pattern: Going in circles
Ignorance Type: Attachment
Illumination Depth: Surface
Illuminated: Modified timeout parameter 3 times in the past
Eliminated: Not a timeout issue
Current Hypothesis: Problem may be in network configuration, not timeout
Next Action: Check network configuration files
```

### Example 2: API Call Failure

**Scenario**: AI says "API call succeeded" but didn't verify

**Trigger**: Verification (empty completion)

**Illumination Process**:
```
[JUE-Illumination Report]
Failure Pattern: Empty completion
Ignorance Type: Complacency
Illumination Depth: Deep
Illuminated: Did not run curl to verify API response
Eliminated: Code looks correct
Current Hypothesis: API may have returned error status code
Next Action: Run curl to verify actual response
```

---

## FAQ

### Q1: Will JUE-AI affect AI performance?

**A**: No. JUE-AI only triggers during failures and does not affect performance under normal conditions. In fact, it improves efficiency by reducing repetitive errors.

### Q2: How to determine illumination depth?

**A**: Automatically determined by failure count:
- 2nd failure → Surface
- 3rd failure → Deep
- 4th failure → Root
- 5th+ failure → Empty

### Q3: Can I customize illumination methods?

**A**: Yes. You can modify the Seven Awakenings checklist in `SKILL.md` to add illumination methods suitable for your scenarios.

### Q4: Which AI frameworks are supported?

**A**: Theoretically supports all AI frameworks that can load Markdown skill files. Tested frameworks:
- Claude Code ✅
- Cursor ✅
- Continue ✅
- Other Markdown skill-supporting frameworks ✅

### Q5: How to contribute new illumination methods?

**A**: Please refer to the [Contributing Guide](#contributing) and submit a Pull Request.

---

## Contributing

We welcome all forms of contribution!

### How to Contribute

1. **Fork this repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Submit a Pull Request**

### Contribution Types

- 🐛 Bug fixes
- ✨ New features
- 📝 Documentation improvements
- 🌍 Translations
- 💡 New ideas

### Code Standards

- Follow Markdown best practices
- Keep documentation concise and clear
- Add necessary examples

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

### Sources of Inspiration

- **Buddhist Consciousness-Only Philosophy**: Three Poisons (greed, hatred, delusion) theory
- **Taoist Thought**: Wu wei (non-action), supreme goodness is like water
- **Zen Wisdom**: Illumination, sudden enlightenment
- **Confucian Classics**: Self-reflection three times a day

### Special Thanks

Thanks to all friends who contributed ideas and suggestions to this project!

---

## Contact

- **GitHub Issues**: [Submit an issue](https://github.com/kscz0000/JUE-AI/issues)
- **GitHub Discussions**: [Join the discussion](https://github.com/kscz0000/JUE-AI/discussions)

---

<div align="center">

**Seeing is the beginning of resolution.**

**Illumination is liberation.**

**If this project helps you, please give it a ⭐ Star!**

</div>
