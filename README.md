# Drucker Skill for AI Agents：将德鲁克思维注入你的本地终端

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![AI Framework](https://img.shields.io/badge/AI_Agent-Claude_Code%20%7C%20OpenClaw-orange)](#)
[![Management](https://img.shields.io/badge/Methodology-Peter_Drucker-success)](#)

Welcome to the **Drucker Skill** repository. This is an open-source AI Agent Skill designed to integrate Peter Drucker's management frameworks into local LLM CLIs (like Claude Code, OpenClaw, and Gemini CLI). 

**Drucker Skill** 是一款专为 AI Agent 设计的底层思维插件。它能约束并引导大语言模型（LLM），使其在为你提供技术架构建议、业务流程诊断或个人决策时，严格遵循彼得·德鲁克的经典管理学逻辑。让你的 AI 从“单纯的代码生成器”进化为“具备顶级商业视角的决策大脑”。

## 🧠 核心注入框架

本 Skill 深度提取并结构化了德鲁克两部核心著作的诊断逻辑：

* **《创新与企业家精神》（Innovation and Entrepreneurship）**
  * **不协调事件诊断**：识别系统假设与现实数据之间的断层。
  * **流程需求分析（Process Need）**：寻找业务流转与架构链路中缺失的关键拼图。
  * ...
* **《卓有成效的管理者》（The Effective Executive）**
  * **决策七原则检验**：防止“头痛医头”的战术勤奋，直击问题根本。
  * **时间与效能审计**：基于目标导向的资源分配诊断。
  * ...

## 🚀 安装与加载

Drucker Skill 设计为轻量级的 Context/Skill 库，支持主流本地 AI 终端。

### 在 AI Cli 中使用（推荐）

1. 将本仓库克隆到本地机器：

   告诉AI Cli仓库地址，自动进行安装，可在Claude code，Gemini Cli等工具中使用。
```bash
git clone [https://github.com/t800code/drucker-skill.git](https://github.com/t800code/drucker-skill.git)
```

2. 将 `SKILL.md` 配置到 Claude Code 的技能目录：
将仓库内的 `SKILL.md` 链接或复制到 `~/.claude/skills/` 目录下。

3. 在终端中唤醒 Drucker 顾问：
```bash
> /skill drucker
```

## 💡 实战使用场景与 Prompt 示例

成功加载 Drucker Skill 后，你可以用以下方式向 AI 发出指令：

**场景一：复杂 IT 架构与流程诊断（Process Need）**
> "调用 Drucker Skill，帮我分析当前这个包含 5 个微服务的 API 链路。不要直接给我重构代码，请用德鲁克的『流程需求』框架，找出那个导致整体延迟极高的 Missing Link。"

**场景二：业务战略与创新机会识别**
> "基于我的系统日志和近期用户反馈（已作为上下文提供），使用 Drucker Skill 寻找『不协调事件』。目前我们的资源投入是否在解决正确的问题？"

**场景三：团队与个人效能复盘**
> "运行 Drucker Skill 中的『卓有成效』模块，审视我这周的 GitHub 提交记录和日历安排，评估我是否将大部分时间花在了产生实际效益的事情上。"

## 📂 仓库目录结构

```text
drucker-skill/
├── SKILL.md                  # 核心系统指令与触发文件
├── references/               # 德鲁克结构化知识库（Context库）
│   ├── 创业与创新/
│   │   ├── 第一章-系统的企业家精神.md
│   │   ├── 第二章-有目的的创新和七个创新机会源.md
│   │   └── 第x章-xxx.md
│   └── 卓有成效的管理者/
│       ├── 第一章-卓有成效可以学会.md
│       └── xxx.md
├── README.md
├── .gitignore
└── LICENSE                   # MIT 开源协议
```

## 🛠️ 维护与共建指南

我们欢迎所有对管理学与 AI 结合感兴趣的开发者参与共建。

**如何添加新的德鲁克认知模型？**
1. 在 `references/` 对应目录下创建新的 `.md` 文件。
2. 遵循结构化格式编写：核心观点提取 -> 诊断触发条件 -> 检查清单 (Checklist)。
3. 同步更新 `SKILL.md` 的索引路由，以确保 AI 能够正确检索到新知识。

```bash
# 提交你的增强型思维模型
git add .
git commit -m "feat: add chapter 5 process need framework"
git push origin main
```

## 📖 参考资料

* 彼得·德鲁克，《创新与企业家精神》
* 彼得·德鲁克，《卓有成效的管理者》

---
*If this skill helps you make better decisions, please consider giving it a ⭐ on GitHub!*