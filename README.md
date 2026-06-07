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
