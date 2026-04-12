# Drucker Skill — 德鲁克管理学 AI 顾问

> 融合《创新与企业家精神》与《卓有成效的管理者》两大核心框架的 Claude Code Skill

## 简介

Drucker Skill 是一款基于彼得·德鲁克（Peter F. Drucker）管理哲学的 AI 顾问工具，帮助你在管理决策、创新机会识别和有效性提升方面获得德鲁克式的深度洞察。

## 核心框架

- **《创新与企业家精神》**：系统化的企业家精神、创新机遇七来源、创新七原则
- **《卓有成效的管理者》**：卓有成效的五项习惯、有效决策七原则

## 在 Claude Code 中加载

### 方法一：Skill 命令（推荐）

```
/skill drucker
```

### 方法二：直接使用 SKILL.md

Claude Code 会自动识别 `~/.claude/skills/` 目录下的 Skill。

## 目录结构

```
drucker-skill/
├── SKILL.md                  # 核心指令文件
├── references/               # 德鲁克精华笔记
│   ├── 创业与创新/
│   │   ├── 第一章-系统的企业家精神.md
│   │   ├── 第二章-有目的的创新和七个创新机会源.md
│   │   └── 第四章-不协调事件.md
│   └── 卓有成效的管理者/
│       └── 第一章-卓有成效可以学会.md
├── README.md
├── .gitignore
└── LICENSE
```

## 使用场景

1. **管理问题诊断** — 使用德鲁克框架分析问题根源
2. **创新机会识别** — 按七个来源系统寻找机会
3. **决策质量提升** — 应用有效决策原则检验决策
4. **时间效能管理** — 德鲁克式时间管理诊断
5. **用人所长咨询** — 识别并发挥个人/团队长处

## 维护指南

### 添加新章节笔记

在 `references/` 对应目录下创建新的 `.md` 文件，格式：

```markdown
# 第X章：章节名称

【待补充德鲁克精华笔记】

## 核心观点

## 案例摘录

## 我的理解与应用
```

### 更新 SKILL.md

如需扩展核心框架或添加新的德鲁克著作章节，请同步更新 `SKILL.md`。

## GitHub 维护

```bash
# 初始化
git init
git add .
git commit -m "feat: initial drucker-skill"

# 推送
git remote add origin https://github.com/YOUR_USERNAME/drucker-skill.git
git push -u origin main
```

## 推荐仓库名称

- `drucker-skill` — 简洁明了
- `drucker-ai-advisor` — 强调 AI 顾问定位
- `personal-drucker-skill` — 个人维护风格

## 参考资料

- 彼得·德鲁克.《创新与企业家精神》
- 彼得·德鲁克.《卓有成效的管理者》

## License

MIT
