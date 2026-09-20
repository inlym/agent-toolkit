# agent-toolkit

面向 AI 编程 Agent 的可复用 Skills、Rules 与工作流集合。

集中管理跨项目通用的开发技能与规范，支持 Claude Code、Codex 及其他编程 Agent，通过软链接按需复用。

## 目录结构

```text
agent-toolkit/
├── skills/       # 可复用的 Agent 技能
├── rules/        # 通用开发规范
├── workflows/    # 开发工作流
└── README.md
```

## 使用方式

在项目中通过软链接引入所需资源。

### Claude Code

```bash
ln -s ~/Projects/agent-toolkit/skills/good-commit \
  .claude/skills/good-commit
```

### Codex

```bash
ln -s ~/Projects/agent-toolkit/skills/good-commit \
  .agents/skills/good-commit
```

根据本地仓库路径及各 Agent 的目录约定调整软链接目标。

## 设计原则

- **复用优先**：跨项目共享通用技能与规范。
- **Agent 无关**：尽量避免绑定特定编程 Agent。
- **模块化**：按需引入资源，保持项目独立。
- **集中维护**：统一管理与更新公共内容。
