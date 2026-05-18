# Agent Instructions

This file is the default entrypoint for AI coding agents working in this repository.

## Collaboration Goal

Help maintain a small, readable, reusable template for AI coding context. Prioritize clarity, low ceremony, and practical reuse over broad documentation.

## Default Behavior

- Read `README.md` first to understand the repository purpose.
- Read the relevant SOP before executing a task.
- Keep changes focused on the user's request.
- Prefer small, explicit edits over broad restructuring.
- Preserve the minimal template shape unless there is a concrete need to evolve it.
- Explain important trade-offs briefly when behavior or structure changes.

## Task Flow

For non-trivial tasks, follow `sop/task-intake.md`:

1. Identify the task goal.
2. Extract constraints and success criteria.
3. Check whether required context is missing.
4. Break the work into a short roadmap.
5. Execute only after the path is clear.
6. Report what changed and how it was verified.

## Output Style

- Be direct and specific.
- Use concise Markdown.
- Lead with results when reporting completed work.
- Include file paths and commands when they help the user verify the work.
- Avoid generic motivational language and vague summaries.

## Boundaries

- Do not add future-facing directories without a documented trigger from `evolution/template-roadmap.md`.
- Do not place private project knowledge in this public template.
- Do not turn `AGENTS.md` into a full project manual.
- Do not duplicate SOP content here; link to the relevant SOP instead.
- Do not invent build, test, or deployment commands. Mark unknown commands as project-specific until confirmed.

## Common Commands

This template does not require a build step.

Project-specific repositories created from this template should fill in commands such as:

```sh
# install dependencies

# run tests

# run linting

# start local development
```

## Reference Documents

- `sop/README.md` for SOP authoring rules.
- `sop/task-intake.md` for task intake and execution.
- `evolution/template-roadmap.md` for deciding when the template should grow.

