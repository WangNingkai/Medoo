```markdown
# Medoo Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development practices for the Medoo codebase, a TypeScript project with a focus on clear code structure and disciplined update workflows. You'll learn the project's coding conventions, how to update core logic with or without tests, and the commands used to streamline contributions.

## Coding Conventions

- **File Naming:**  
  Use PascalCase for file names.  
  _Example:_  
  ```
  DataMapTest.ts
  MedooCore.ts
  ```

- **Import Style:**  
  Use relative imports.  
  _Example:_  
  ```typescript
  import { DataMap } from './DataMap';
  ```

- **Export Style:**  
  Use named exports.  
  _Example:_  
  ```typescript
  export function mapColumn() { ... }
  export const DEFAULTS = { ... };
  ```

- **Commit Messages:**  
  - Freeform style, often prefixed with `[update]`.
  - Average commit message length: ~39 characters.
  _Example:_  
  ```
  [update] Improve column mapping logic
  ```

## Workflows

### Core Logic Update with Related Tests
**Trigger:** When you want to improve or fix core logic and ensure changes are covered by tests.  
**Command:** `/update-core-with-tests`

1. Edit `src/Medoo.php` to implement your improvement or fix.
2. Update or add relevant test files in `tests/` (e.g., `DataMapTest.php`, `ColumnMappingTest.php`) to cover your changes.
3. Commit both the implementation and test changes together.

_Example commit message:_  
```
[update] Refactor query builder and add coverage in DataMapTest
```

### Core Logic Update Without Tests
**Trigger:** When making a small or isolated improvement/fix to the core logic that does not require test changes.  
**Command:** `/update-core`

1. Edit `src/Medoo.php` to implement your improvement or fix.
2. Commit the change without touching any test files.

_Example commit message:_  
```
[update] Optimize connection pooling
```

## Testing Patterns

- **Framework:** Unknown (not detected)
- **Test File Pattern:** Files matching `*.test.*` (e.g., `DataMapTest.php`)
- **Test Location:** All test files are located in the `tests/` directory.
- **Best Practice:** When updating core logic, add or update tests to ensure correctness and performance, unless the change is trivial or isolated.

_Example test file:_  
```
tests/DataMapTest.php
```

## Commands

| Command                  | Purpose                                                        |
|--------------------------|----------------------------------------------------------------|
| /update-core-with-tests  | Update core logic and related tests together                   |
| /update-core             | Update core logic without modifying tests                      |
```
