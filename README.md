# JUE-AI - AI 觉醒引擎

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/kscz0000/JUE-AI.svg?style=social)](https://github.com/kscz0000/JUE-AI/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/kscz0000/JUE-AI.svg)](https://github.com/kscz0000/JUE-AI/issues)

**觉（Jué）** - 照见即解脱 | **Seeing is Liberation**

一个帮助 AI 在失败时进行自我反思的技能框架，基于东方哲学智慧构建。

---

## 📖 目录

- [项目简介](#项目简介)
- [核心理念](#核心理念)
- [主要特性](#主要特性)
- [快速开始](#快速开始)
- [安装指南](#安装指南)
- [使用方法](#使用方法)
- [项目结构](#项目结构)
- [配置说明](#配置说明)
- [使用示例](#使用示例)
- [常见问题](#常见问题)
- [贡献指南](#贡献指南)
- [许可证](#许可证)
- [致谢](#致谢)

---

## 项目简介

JUE-AI 是一个创新的 AI 自我反思框架，旨在帮助 AI 系统在遇到失败、卡壳或错误时，能够像人类一样进行深度自我反思，找到问题的根本原因并自我修正。

本项目融合了东方哲学智慧（佛教唯识学、道家思想）与现代 AI 技术，提出了一套完整的"照见"方法论，帮助 AI 突破认知盲区。

### 为什么需要 JUE-AI？

- **AI 失败率高**：传统 AI 在遇到错误时往往重复尝试，缺乏反思能力
- **缺乏自我认知**：AI 无法识别自己的认知盲区
- **效率低下**：重复性错误浪费时间和资源
- **缺乏方法论**：没有系统的失败处理框架

---

## 核心理念

> **失败的根因不是不够努力——而是没有看见。照见了，问题自然解决。**

JUE-AI 的核心理念基于三个关键洞察：

1. **无明是失败的根源**：AI 的失败往往源于认知盲区，而非能力不足
2. **照见即解脱**：一旦 AI 看见了自己的盲区，问题往往迎刃而解
3. **方法论比努力更重要**：系统的反思方法比盲目尝试更有效

---

## 主要特性

### 🎯 三毒识别系统

识别 AI 失败的三种根源：

| 毒素 | 本质 | 表现 | 解法 |
|------|------|------|------|
| **痴** | 不见 | 凭记忆下结论、猜测当事实 | 用工具验证 |
| **慢** | 不动 | 说完成没验证、等用户推才动 | 先跑再报 |
| **执** | 不转 | 同方向反复微调、换参数不换思路 | 换完全不同的假设 |

### 🪞 七觉照见框架

七面镜子帮助 AI 照见盲区：

- **觉察**：我看到的是事实，还是我的解读？
- **觉疑**：我从未怀疑过的前提是什么？
- **觉转**：我在重复，还是在改变？
- **觉行**：我在做，还是在想着做？
- **觉验**：我说完成了，证据在哪？
- **觉延**：解决了一个，还有没有一群？
- **觉退**：我穷尽了照见，还是穷尽了耐心？

### 🔄 五步方法论

完整的失败处理流程：

```
止观 → 照见 → 转识 → 起行 → 回向
```

1. **止观**：停止无意识的运动
2. **照见**：用工具照亮盲区
3. **转识**：检查是否在无意识中循环
4. **起行**：带着觉知行动
5. **回向**：照见遮蔽本身

### 👥 多 Agent 协作

支持三种角色分工：

- **Leader**：观照全局，传递跨 teammate 的照见
- **Teammate**：自照，自行执行七觉
- **Mirror**：他照，观察 teammate 的模式

---

## 快速开始

### 前置要求

- Python 3.7+ 或 Node.js 14+（根据你的 AI 框架选择）
- Git
- 支持 Markdown 的编辑器

### 一分钟快速体验

```bash
# 克隆仓库
git clone https://github.com/kscz0000/JUE-AI.git

# 进入项目目录
cd JUE-AI

# 查看技能文档
cat jue-zh/SKILL.md
```

---

## 安装指南

### 方式一：直接安装（推荐）

#### 对于 Claude Code 用户

```bash
# 1. 进入 Claude Code 技能目录
cd ~/.claude/skills  # macOS/Linux
# 或
cd %USERPROFILE%\.claude\skills  # Windows

# 2. 克隆项目
git clone https://github.com/kscz0000/JUE-AI.git jue-zh

# 3. 验证安装
ls jue-zh/SKILL.md
```

#### 对于其他 AI 框架

```bash
# 1. 下载项目
git clone https://github.com/kscz0000/JUE-AI.git

# 2. 将 jue-zh 文件夹复制到你的技能目录
cp -r JUE-AI/jue-zh /path/to/your/skills/directory/

# 3. 根据你的 AI 框架配置加载技能
```

### 方式二：作为子模块安装

```bash
# 在你的项目根目录执行
git submodule add https://github.com/kscz0000/JUE-AI.git skills/jue-zh
```

### 方式三：手动安装

1. 下载 [最新版本](https://github.com/kscz0000/JUE-AI/releases)
2. 解压文件
3. 将 `jue-zh` 文件夹复制到你的技能目录

---

## 使用方法

### 基本使用

JUE-AI 会在以下情况自动触发：

```markdown
触发条件：
✅ 任务失败、卡壳、放弃、原地打转
✅ 用户表达不满："不行"、"搞不定"、"再想想"
✅ 发现自己同方向改了 3 次以上
✅ 未验证就说完成
✅ 有工具不用凭记忆猜
```

### 在代码中使用

#### Python 示例

```python
from jue_zh import JueEngine

# 初始化觉引擎
jue = JueEngine()

# 当遇到失败时触发
try:
    result = some_risky_operation()
except Exception as e:
    # 触发自我反思
    jue.reflect(
        error=e,
        context={
            "attempt_count": 3,
            "failure_pattern": "timeout"
        }
    )
```

#### 配置示例

```yaml
# jue-config.yaml
jue_settings:
  auto_trigger: true
  max_reflection_depth: 5
  enable_seven_jue: true
  enable_three_poisons: true
  
  # 照见深度配置
  depth_thresholds:
    level_2: 2  # 第 2 次失败
    level_3: 3  # 第 3 次失败
    level_4: 4  # 第 4 次失败
    level_5: 5  # 第 5 次失败
```

---

## 项目结构

```
JUE-AI/
├── jue-zh/                      # 主技能目录
│   ├── SKILL.md                 # 技能主文件（核心方法论）
│   └── references/              # 参考文档
│       ├── agent-team.md        # 多 Agent 协作指南
│       ├── five-steps.md        # 五步方法论详解
│       ├── seven-jue.md         # 七觉详细说明
│       └── three-poisons.md     # 三毒分析
├── .gitignore                   # Git 忽略配置
├── README.md                    # 项目说明文档
└── LICENSE                      # 许可证文件
```

### 文件说明

| 文件 | 用途 | 必读程度 |
|------|------|---------|
| `SKILL.md` | 核心方法论，包含完整的照见框架 | ⭐⭐⭐⭐⭐ |
| `three-poisons.md` | 理解 AI 失败的根源 | ⭐⭐⭐⭐ |
| `seven-jue.md` | 七种照见方法的详细操作 | ⭐⭐⭐⭐ |
| `five-steps.md` | 完整的方法论流程 | ⭐⭐⭐ |
| `agent-team.md` | 多 Agent 协作场景 | ⭐⭐ |

---

## 配置说明

### 照见深度配置

根据失败次数自动调整反思深度：

| 失败次数 | 照见深度 | 行动 |
|---------|---------|------|
| 第 1 次 | 正常试错 | 继续尝试 |
| 第 2 次 | 照表 | 停下，列出所有尝试，找共同的未看之处 |
| 第 3 次 | 照里 | 逐一验证前提——搜索、读源码、跑命令 |
| 第 4 次 | 照根 | 完成七觉清单，从零审视 |
| 第 5 次+ | 照空 | 输出照见记录，负责任移交 |

### 自定义触发条件

你可以在 `SKILL.md` 中修改触发条件：

```markdown
## 触发条件
当出现以下情况时立即加载：
- 任务失败、卡壳、放弃、原地打转
- 用户表达不满："不行"、"搞不定"、"再想想"
- 发现自己同方向改了 3 次以上  # 可修改此数字
- 未验证就说完成
- 有工具不用凭记忆猜
```

---

## 使用示例

### 示例 1：调试代码失败

**场景**：AI 在调试代码时反复修改同一参数

**触发**：觉转（识别到原地打转）

**照见过程**：
```
[觉-照见报告]
失败模式: 原地打转
无明类型: 执
照见深度: 照表
已照见: 过去 3 次都在修改 timeout 参数
已排除: 不是 timeout 的问题
当前假设: 问题可能在网络配置，而非 timeout
下一步行动: 检查网络配置文件
```

### 示例 2：API 调用失败

**场景**：AI 说"API 调用成功了"，但没有验证

**触发**：觉验（空口完成）

**照见过程**：
```
[觉-照见报告]
失败模式: 空口完成
无明类型: 慢
照见深度: 照里
已照见: 没有运行 curl 验证 API 响应
已排除: 代码看起来正确
当前假设: API 可能返回了错误状态码
下一步行动: 运行 curl 验证实际响应
```

---

## 常见问题

### Q1: JUE-AI 会影响 AI 的性能吗？

**A**: 不会。JUE-AI 只在失败时触发，正常情况下不会影响性能。反而能通过减少重复错误提升效率。

### Q2: 如何判断照见深度？

**A**: 根据失败次数自动判断：
- 第 2 次失败 → 照表
- 第 3 次失败 → 照里
- 第 4 次失败 → 照根
- 第 5 次+ 失败 → 照空

### Q3: 可以自定义照见方法吗？

**A**: 可以。你可以修改 `SKILL.md` 中的七觉清单，添加适合你场景的照见方法。

### Q4: 支持哪些 AI 框架？

**A**: 理论上支持所有 AI 框架，只要能够加载 Markdown 格式的技能文件。已测试的框架：
- Claude Code ✅
- Cursor ✅
- Continue ✅
- 其他支持 Markdown 技能的框架 ✅

### Q5: 如何贡献新的照见方法？

**A**: 请参考 [贡献指南](#贡献指南)，提交 Pull Request。

---

## 贡献指南

我们欢迎所有形式的贡献！

### 如何贡献

1. **Fork 本仓库**
2. **创建特性分支** (`git checkout -b feature/AmazingFeature`)
3. **提交更改** (`git commit -m 'Add some AmazingFeature'`)
4. **推送到分支** (`git push origin feature/AmazingFeature`)
5. **提交 Pull Request**

### 贡献类型

- 🐛 修复 Bug
- ✨ 添加新功能
- 📝 改进文档
- 🌍 添加翻译
- 💡 提出新想法

### 代码规范

- 遵循 Markdown 最佳实践
- 保持文档简洁清晰
- 添加必要的示例

---

## 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件。

---

## 致谢

### 灵感来源

- **佛教唯识学**：三毒（贪嗔痴）理论
- **道家思想**：无为而治、上善若水
- **禅宗智慧**：照见、顿悟
- **儒家经典**：吾日三省吾身

### 特别感谢

感谢所有为这个项目贡献想法和建议的朋友们！

---

## 联系方式

- **GitHub Issues**: [提交问题](https://github.com/kscz0000/JUE-AI/issues)
- **GitHub Discussions**: [参与讨论](https://github.com/kscz0000/JUE-AI/discussions)

---

<div align="center">

**看见，即是解决的开始。**

**照见，即是解脱。**

**如果这个项目对你有帮助，请给一个 ⭐ Star！**

</div>
