# AI Context Template

A minimal GitHub template for AI coding context, project instructions, SOPs, and future workflow documentation.

This repository is not a general documentation archive. It is a small, reusable starting point for projects that need a clear collaboration entrypoint for humans and AI coding tools.

## Use Cases

Use this template when you want to:

- Give AI coding tools a stable project entrypoint.
- Keep human-facing project context and AI-facing rules close together.
- Start with a small structure that can grow only when real patterns appear.
- Reuse the same collaboration habits across private or public projects.

## Quick Start

1. Create a new repository from this template.
2. Update this `README.md` with the new project's purpose and setup notes.
3. Update `AGENTS.md` with project-specific commands, boundaries, and tool expectations.
4. Review `sop/task-intake.md` before asking an AI tool to execute a non-trivial task.
5. Use `evolution/template-roadmap.md` to decide when the template should grow.

## Files

| Path | Purpose |
| --- | --- |
| `README.md` | Human-facing project overview and usage guide. |
| `AGENTS.md` | AI-facing collaboration rules and execution guidance. |
| `sop/README.md` | Rules for writing and maintaining SOP documents. |
| `sop/task-intake.md` | The first SOP for receiving, clarifying, planning, and executing tasks. |
| `evolution/template-roadmap.md` | Guidance for evolving the template without over-designing it. |

## Template Usage

After creating a repository from this template, replace generic placeholders before starting real work:

- Project name and purpose.
- Build, test, lint, and run commands.
- Required environment variables or setup steps.
- Project-specific constraints for AI tools.
- Any local SOPs that are already known to be useful.

Do not add directories just because they might be useful later. Add them when repeated work creates a clear need.

## Evolution Principles

- Keep the structure small until the project has repeated patterns.
- Prefer one clear document over several shallow documents.
- Treat SOPs as reusable operating procedures, not essays.
- Move stable rules into dedicated standards only after they repeat across tasks.
- Add examples only when rules alone do not produce consistent output.

