# Its Wrap Skill  活干完了！

[English](README.md) | 中文版

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> 将研究转化为决策。一个帮助研究人员与产品经理沟通的 Claude Code Skill。

将研究内容转化为可执行的决策资产，加速从理论到工程的转变。现在，去把那些材料甩给那个永远不知足的产品经理吧！

## 快速开始

```bash
git clone https://github.com/Gh0se4/its-wrap-skill.git
cp -r its-wrap-skill/.skill ~/.claude/skills/its-wrap
```

然后在 Claude Code 中说：*"我有一个研究 demo，帮我把它转成产品决策包。"*

## 它是什么

Its Wrap 架起了**研究完成**到**产品决策**之间的桥梁。

研究人员经常有可行的 demo、原型或实验，显示出潜力——但将这些工作转化为产品经理可以评估和行动的内容却很难。

这个 Skill 结构化了这个转换过程。

## 何时使用

| 你有... | 使用 Its Wrap 当... |
|-------------|---------------------|
| 可用的 demo | 你需要将其呈现给 PM 评估 |
| Vibe-coded 原型 | 你想识别哪些部分可投产、哪些该丢弃 |
| LLM/AI 实验 | 你需要结构化证据和验证计划 |
| 算法改进 | 你想将技术收益映射到用户价值 |
| 研究笔记 | 你需要将其整理成决策包 |

## 它产出什么

一个结构化的交付包，涵盖：

1. **执行摘要** — 快速决策建议
2. **问题与用户场景** — 为什么重要
3. **研究资产** — 当前有什么
4. **产品化方案** — 它可以变成什么
5. **决策证据** — 已验证的 vs 假设的
6. **不可量化价值** — 战略/体验价值
7. **替代方案** — 考虑的更简单选项
8. **落地路径** — 如何从这里到上线
9. **成本模型** — 开发和运营成本
10. **风险与边界** — 可能出错的地方
11. **数据闭环** — 如何衡量和改进
12. **缺失信息** — 需要填补的已知缺口
13. **下一步行动** — 具体的建议步骤

## 安装

详见 [INSTALL.md](INSTALL.md)。

### 快速安装

```bash
# 克隆仓库
git clone https://github.com/Gh0se4/its-wrap-skill.git

# 安装到 Claude Code
mkdir -p ~/.claude/skills
cp -r its-wrap-skill/.skill ~/.claude/skills/its-wrap

# 重启 Claude Code
```

## 使用

详见 [USAGE.md](USAGE.md)。

### 基本用法

描述你的研究并请求产品决策交付：

```
"我搭建了一个自动分类客服工单的 LLM demo。
在 200 条历史工单上运行良好。帮我把它转成
PM 可以用来决策下一步的材料。"
```

Claude 会调用 Its Wrap 并生成结构化交付包。

### 处理缺失信息

如果关键信息缺失，Its Wrap 会发起澄清问题：

- "目标用户是谁？"
- "这解决了什么问题？"
- "你有 baseline 指标吗？"

回答这些问题以改进输出，或继续使用标记为 `待补充` 的缺口。

## 核心特性

### 🎯 决策导向

每个输出元素都服务于产品决策。没有废话，没有泛泛的总结。

### 🔍 缺口检测

自动识别会影响决策的缺失信息。

### 🛠️ Vibe-Coding 感知

针对 vibe-coded 原型的特殊处理——区分 demo 质量与可投产质量。

### 🤖 AI/LLM 就绪

包含 AI 研究的特定检查：prompt 结构、评估标准、成本模型、安全考虑。

### ⚖️ 平衡视角

始终呈现替代方案和权衡，而非只有"做它"的情况。

## 文档

| 文件 | 说明 |
|------|-------------|
| [README.md](README.md) | 英文说明 |
| [README.zh-CN.md](README.zh-CN.md) | 本文件 — 中文说明 |
| [INSTALL.md](INSTALL.md) | 详细安装说明 |
| [USAGE.md](USAGE.md) | 使用示例和工作流 |
| [CONTRIBUTING.md](CONTRIBUTING.md) | 如何贡献 |
| [.skill/SKILL.md](.skill/SKILL.md) | 完整 Skill 规范 |

## 理念

Its Wrap 遵循以下原则：

1. **研究员优先** — 服务于与 PM 沟通的研究人员
2. **决策支持** — 准备材料，不做决策
3. **诚实面对缺口** — 始终暴露缺失信息
4. **灵活结构** — 适应输入复杂度，同时保持严谨

## 贡献

欢迎贡献！详见 [CONTRIBUTING.md](CONTRIBUTING.md)。

## 许可证

MIT 许可证 — 详见 [LICENSE](LICENSE)。

## 相关

- [Claude Code](https://claude.ai/code) — 使用此 Skill 的 AI 编程助手
- [Agent Skills Specification](https://agentskills.io) — Agent Skill 标准

---

**用 ❤️ 为希望工作能落地的研究人员而做。**
