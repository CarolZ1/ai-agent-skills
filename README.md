# AI Agent Skills Collection / AI 智能体技能合集

A collection of **8 production-ready AI agent skills** — drop any folder into your agent's skills directory (e.g. `~/.workbuddy/skills/`) and it works.
**8 个可直接使用的 AI 智能体技能**合集——把任意文件夹放入智能体的 skills 目录（如 `~/.workbuddy/skills/`）即可生效。

## Skills / 技能清单

| Skill | 中文名 | What it does / 作用 |
|---|---|---|
| [code-review](https://github.com/CarolZ1/code-review) | 代码审查与质量 | Five-axis code review (correctness, readability, architecture, security, performance) with severity labels… |
| [debugging](https://github.com/CarolZ1/debugging) | 系统化调试 | Four-phase root-cause investigation discipline: no fixes without investigation first, with an escalation rule… |
| [file-organizer](https://github.com/CarolZ1/file-organizer) | 文件整理 | Safety-first file organization: read-only scanning, SHA-256 duplicate detection, recycle-bin-only deletion,… |
| [markitdown](https://github.com/CarolZ1/markitdown) | 文档转 Markdown | Document-to-Markdown skill built on Microsoft MarkItDown 0.1.6: safe local conversion, batch workflows,… |
| [skill-builder](https://github.com/CarolZ1/skill-builder) | Skill 制作器 | Cross-platform skill authoring guide: intent capture, trigger-word writing, structure guide, quality… |
| [skill-reviewer](https://github.com/CarolZ1/skill-reviewer) | Skill 审查器 | Audit and auto-score a skill against an 11-dimension standard, with hard-check scripts (structure compliance,… |
| [tdd](https://github.com/CarolZ1/tdd) | 测试驱动开发 | Red-green-refactor loop discipline with the iron law 'no production code without a failing test first';… |
| [text-patterns](https://github.com/CarolZ1/text-patterns) | 文本处理模式库 | Curated ~50 text-processing patterns from Daniel Miessler's fabric: summarize, extract insights, analyze… |

## What is an agent skill? / 什么是智能体技能

A skill is a folder containing a `SKILL.md` instruction file (plus optional `references/`, `scripts/`, `examples/`) that an AI agent loads on demand. The `description` field in the frontmatter is the trigger: when the user's request matches it, the agent loads the skill and follows its workflow.
技能是一个包含 `SKILL.md` 指令文件的文件夹（可附带 `references/`、`scripts/`、`examples/`），由 AI 智能体按需加载。frontmatter 里的 `description` 就是触发器：当用户请求匹配时，智能体加载该技能并按其中的流程执行。

## Design principles / 设计原则

- **Iron laws over vague advice** — each skill states its non-negotiable rule (e.g. "no fixes without root-cause investigation", "no production code without a failing test"). / **铁律优于泛泛建议**：每个技能都写明不可协商的规则。
- **Safety first** — destructive operations require confirmation, reuse the recycle bin, and back up first. / **安全优先**：破坏性操作需确认、走回收站、先备份。
- **Cross-platform** — Windows / macOS / Linux command equivalents are documented. / **跨平台**：给出三平台等价命令。
- **Bilingual** — every skill ships an English/Chinese README. / **中英双语**：每个技能都附双语 README。
- **Graceful degradation** — when a dependency is missing, the skill falls back instead of failing. / **优雅降级**：缺依赖时降级而非报错。

## Repositories / 仓库列表

- https://github.com/CarolZ1/code-review — Code Review — 代码审查与质量
- https://github.com/CarolZ1/debugging — Systematic Debugging — 系统化调试
- https://github.com/CarolZ1/file-organizer — File Organizer — 文件整理
- https://github.com/CarolZ1/markitdown — MarkItDown Skill — 文档转 Markdown
- https://github.com/CarolZ1/skill-builder — Skill Builder — Skill 制作器
- https://github.com/CarolZ1/skill-reviewer — Skill Reviewer — Skill 审查器
- https://github.com/CarolZ1/tdd — TDD — 测试驱动开发
- https://github.com/CarolZ1/text-patterns — Text Patterns — 文本处理模式库

## License / 许可

Individual skills carry their own license; `code-review`, `debugging` and `tdd` are MIT.
各技能许可以各自仓库为准；`code-review`、`debugging`、`tdd` 为 MIT。

---
Maintained by [CarolZ1](https://github.com/CarolZ1) / 维护者：CarolZ1
