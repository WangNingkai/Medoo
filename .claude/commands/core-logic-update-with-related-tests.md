---
name: core-logic-update-with-related-tests
description: Workflow command scaffold for core-logic-update-with-related-tests in Medoo.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /core-logic-update-with-related-tests

Use this workflow when working on **core-logic-update-with-related-tests** in `Medoo`.

## Goal

Update core logic in src/Medoo.php and update or add related test files to ensure correctness and performance.

## Common Files

- `src/Medoo.php`
- `tests/*.php`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Edit src/Medoo.php to implement the improvement or fix.
- Update or add relevant test files in tests/ (e.g., DataMapTest.php, ColumnMappingTest.php) to cover the changes.
- Commit both the implementation and test changes together.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.