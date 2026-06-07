# Power Electronics Notes Skill

A Claude Code skill for generating publication-ready study notes in LaTeX for power electronics topics.

## What it does

This skill provides a three-stage workflow for creating comprehensive study notes:

1. **Stage 1: Interactive Chinese Discussion** — Deep, conversational explanation in Chinese to build understanding before writing
2. **Stage 2: English LaTeX Notes** — Complete, compilable `.tex` file with professional formatting
3. **Stage 3: Chinese LaTeX Notes** — Translated version using `ctexart` for XeLaTeX/LuaLaTeX compilation

## Content Scope

Not limited to any single textbook. Works with:
- Textbooks (Erickson, Mohan, Basso, Kazimierczuk, etc.)
- IEEE/IET academic papers
- Application notes (TI, Infineon, ROHM, STMicro, etc.)
- Course materials, lab manuals, datasheets

## Installation

Clone this repo into your Claude Code skills directory:

```bash
# Global (all projects)
git clone https://github.com/Franz-V/power-electronics-notes-skill.git ~/.claude/skills/power-electronics-notes

# Project-level (single project)
git clone https://github.com/Franz-V/power-electronics-notes-skill.git .claude/skills/power-electronics-notes
```

## Usage

The skill triggers automatically when you:
- Upload textbook pages and ask for notes
- Mention converter topologies (buck, boost, flyback, DAB, etc.)
- Say "generate notes", "Stage 1/2/3", "笔记", "帮我整理"

Or invoke manually: reference the three-stage workflow in your message.

## Output

- `main_en.tex` — English notes (pdfLaTeX)
- `main_cn.tex` — Chinese notes (XeLaTeX / LuaLaTeX)

## Template Features

- `noteblue` color scheme with `\blue{}` command for key insights
- `keybox` environment for fundamental principles
- `figbox` environment for figure placeholders
- Professional headers/footers with `fancyhdr`
- Numbered equations with `\boxed{}` for critical results

## Author

Study Notes By Catastrophy_ame

---

## 中文说明

一个用于生成电力电子学 LaTeX 学习笔记的 Claude Code Skill。

### 功能简介

本 Skill 提供三阶段工作流，帮你从阅读材料生成高质量的中英文学习笔记：

1. **Stage 1：中文互动讨论** — 先用中文深入讲解，构建理解，不急着写 LaTeX
2. **Stage 2：英文 LaTeX 笔记** — 生成完整可编译的 `.tex` 文件，排版专业
3. **Stage 3：中文 LaTeX 笔记** — 翻译为中文版，使用 `ctexart` 文档类，需 XeLaTeX/LuaLaTeX 编译

### 适用范围

不限于某一本教材，支持任何电力电子相关内容：
- 教材（Erickson、Mohan、Basso、Kazimierczuk 等）
- IEEE/IET 学术论文
- 应用笔记（TI、Infineon、ROHM、STMicro 等）
- 课程资料、实验手册、数据手册

### 安装方法

将本仓库克隆到 Claude Code 的 skills 目录：

```bash
# 全局安装（所有项目可用）
git clone https://github.com/Franz-V/power-electronics-notes-skill.git ~/.claude/skills/power-electronics-notes

# 项目级安装（仅当前项目）
git clone https://github.com/Franz-V/power-electronics-notes-skill.git .claude/skills/power-electronics-notes
```

### 使用方式

Skill 会在以下情况自动触发：
- 上传教材页面并要求生成笔记
- 提到变换器拓扑（buck、boost、flyback、DAB 等）
- 说 "generate notes"、"Stage 1/2/3"、"笔记"、"帮我整理"

### 输出文件

- `main_en.tex` — 英文笔记（pdfLaTeX 编译）
- `main_cn.tex` — 中文笔记（XeLaTeX / LuaLaTeX 编译）

### 模板特性

- `noteblue` 配色方案，`\blue{}` 命令高亮关键结论
- `keybox` 环境用于基本原理和公式总结
- `figbox` 环境用于图片占位
- `fancyhdr` 专业页眉页脚
- 重要公式使用 `\boxed{}` 加框
