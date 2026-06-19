---
name: core-logic-update-no-tests
description: Workflow command scaffold for core-logic-update-no-tests in Medoo.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /core-logic-update-no-tests

Use this workflow when working on **core-logic-update-no-tests** in `Medoo`.

## Goal

Update core logic in src/Medoo.php without modifying any test files.

## Common Files

- `src/Medoo.php`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Edit src/Medoo.php to implement the improvement or fix.
- Commit the change without touching any test files.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.