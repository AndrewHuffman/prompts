---
trigger: model_decision
description: This rule explains how to create new .md project rule files for the Windsurf agent.
---

# Windsurf Rules Location

How to add new windsurf rules to the project

1. Always place rule files in PROJECT_ROOT/windsurf/:
    ```
    windsurf/
    ├── your-rule-name.md
    ├── another-rule.md
    └── ...
    ```

2. Follow the naming convention:
    - Use kebab-case for filenames
    - Always use .md extension
    - Make names descriptive of the rule's purpose

3. Directory structure:
    ```
    PROJECT_ROOT/
    ├── windsurf/
    │   ├── your-rule-name.md
    │   └── ...
    └── ...
    ```

4. Never place rule files:
    - In the project root
    - In subdirectories outside windsurf/
    - In any other location

5. Windsurf rules have the following structure:

```
---
trigger: model_decision
description: Short description of the rule's purpose
---
# Rule Title

Main content explaining the rule with markdown formatting.

1. Step-by-step instructions
2. Code examples
3. Guidelines

Example:
```typescript
// Good example
function goodExample() {
  // Implementation following guidelines
}

// Bad example
function badExample() {
  // Implementation not following guidelines
}
```
```

## Key Points

- Rules are stored as `.md` files in the `windsurf/` directory
- All rules use `trigger: model_decision` in frontmatter
- Content should be clear, actionable guidelines
- Include examples when helpful
- Use descriptive filenames that reflect the rule's purpose
