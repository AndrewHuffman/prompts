---
trigger: model_decision
description: This rule explains how to create and update an analytics.md file to track how often .md rules are being used.
---

# Windsurf Rules Analytics

Each time you use a Windsurf rule, update the analytics tracking file.

File location:
```
PROJECT_ROOT/windsurf/analytics.md
```

## Format

The analytics file contains a count of how many times each rule has been used:

```
rule-name.md: 5
another-rule.md: 2
```

Add new rules as needed.
