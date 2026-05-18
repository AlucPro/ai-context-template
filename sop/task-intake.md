# Task Intake SOP

## Purpose

Use this SOP to receive a task, understand the desired outcome, and create a clear execution path before making changes.

## When To Use

Use this SOP for any task that is more than a direct one-command answer. It is especially useful for feature work, documentation changes, repository setup, debugging, refactoring, and review requests.

## Inputs

- User request.
- Existing repository files.
- Relevant project instructions such as `AGENTS.md`.
- Any referenced specification, issue, design note, or external requirement.

## Steps

1. Identify the goal.
   - Restate what the user wants in concrete terms.
   - Separate the desired outcome from implementation assumptions.

2. Extract constraints.
   - Note required files, formats, commands, style rules, deadlines, and forbidden changes.
   - Check whether the task must preserve existing structure or behavior.

3. Check for missing information.
   - If a reasonable default is safe, choose it and continue.
   - If the missing detail could change the result materially, ask one focused question.

4. Inspect the current state.
   - Read the relevant files before editing.
   - Check whether there are uncommitted changes.
   - Avoid overwriting unrelated user work.

5. Create a short roadmap.
   - Break the task into the smallest useful steps.
   - Include verification before calling the task complete.
   - Keep the roadmap proportional to the task size.

6. Execute the roadmap.
   - Make focused edits.
   - Follow existing project patterns.
   - Avoid adding future-facing structure unless the task explicitly requires it.

7. Verify the result.
   - Run the relevant checks when available.
   - For documentation-only changes, verify required files, headings, links, and stated constraints.

8. Report the outcome.
   - Summarize what changed.
   - Include verification results.
   - Mention any remaining uncertainty or follow-up work.

## Output

A completed task should produce:

- The requested change.
- A concise summary of touched files.
- The verification performed.
- Any important caveats.

## Verification

Before finishing, confirm:

- The result matches the user's stated goal.
- Required files or sections exist.
- The implementation does not add unrelated structure.
- Any commands or checks used are reported accurately.

