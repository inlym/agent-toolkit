---
name: good-commit
description: 自动化 Git 代码提交流程。分析工作区改动，生成符合 Conventional Commit 规范的中文提交消息，将所有修改合并为单次提交并推送到远程仓库，不限定编程语言与技术栈。当用户表达"提交代码"、"commit 代码"、"提交修改"、"推送代码"、"git commit"等提交意图时使用。
allowed-tools: Bash(git status:*), Bash(git diff:*), Bash(git log:*), Bash(git add:*), Bash(git commit:*), Bash(git push:*), Bash(git pull:*)
---

# Git Commit Skill

## 概述

将当前工作区的所有修改内容合并为单次提交并推送到远程仓库。提交消息遵循项目 Git 提交规范（类型前缀 + 范围 + 中文描述），确保清晰、准确。

不限定编程语言与技术栈，适用于任何语言的项目。

## 使用场景

- 完成功能开发后提交代码
- 修复 bug 后提交代码
- 重构代码后提交代码
- 任何需要将代码变更持久化到 Git 仓库的场景

## 执行

收到触发请求后，完整阅读并严格遵循 [instruction.md](./instruction.md) 中的七步执行流程（含消息格式规范、执行原则与错误处理）。
