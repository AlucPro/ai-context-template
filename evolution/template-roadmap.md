# Template Roadmap

This template starts small on purpose. The initial structure should make AI collaboration easier without pretending to know every future project need.

## Current Structure

```txt
ai-context-template/
├── README.md
├── AGENTS.md
├── .gitignore
├── sop/
│   ├── README.md
│   └── task-intake.md
└── evolution/
    └── template-roadmap.md
```

## Why The MVP Is Minimal

- Empty directories create noise.
- Large instruction sets are harder for humans and agents to follow.
- Real usage should drive new structure.
- A template repository should stay easy to copy, inspect, and adapt.

## Add `workflows/`

Add this directory when multiple SOPs need to be composed in a repeatable order.

Examples:

- Feature development.
- Bug fixing.
- Release preparation.

Use `workflows/` for orchestration. Keep individual reusable actions in `sop/`.

## Add `standards/`

Add this directory when stable rules are repeated across tasks.

Examples:

- Naming conventions.
- Git conventions.
- Testing expectations.
- Language-specific style rules.

Use `standards/` for durable constraints, not temporary project notes.

## Add `examples/`

Add this directory when instructions alone do not produce consistent output.

Examples:

- Good task breakdowns.
- Good pull request descriptions.
- Good refactor plans.
- Good review comments.

Examples should be short and representative. They should show the desired shape of work.

## Add `memory/`

Add this directory when long-running projects repeatedly need the same preferences or context.

Examples:

- Architecture preferences.
- Communication preferences.
- Stable product context.
- Team-specific operating habits.

Do not store secrets or sensitive private context in a public template.

## Add `.github/`

Add this directory when GitHub-specific collaboration becomes part of the template.

Examples:

- Copilot instructions.
- Issue templates.
- Pull request templates.
- Repository automation.

Keep GitHub automation out of the MVP until the template has proven its base structure.

## Change Rule

Only evolve the template when a repeated need appears. When adding a new directory, update this roadmap and explain the trigger that justified the addition.

