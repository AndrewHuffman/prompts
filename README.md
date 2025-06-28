# AI Coding Assistant Prompt Rules

A curated collection of prompt rules and templates designed to enhance AI coding assistants' behavior and capabilities. This repository provides structured guidelines for both Cursor and Windsurf AI coding environments.

## Overview

This repository contains specialized prompt rules that help AI coding assistants:
- Maintain consistent coding practices across projects
- Manage project memory and learned preferences
- Create and track task lists effectively
- Generate analytics on rule effectiveness
- Set up proper testing workflows with Vitest

The rules are designed to be trigger-based, activating when specific conditions or decisions need to be made during coding sessions.

## Directory Structure

```
prompts/
├── cursor/          # Cursor-specific prompt files (.mdc format)
├── windsurf/        # Windsurf-specific prompt files (.md format)
└── README.md        # This documentation
```

### File Format Differences
- **Cursor**: Uses `.mdc` (Markdown with Cursor extensions)
- **Windsurf**: Uses standard `.md` (Markdown format)

## Available Rules & Prompts

### Core Rules (Available in both platforms)

| Rule | Purpose | Trigger |
|------|---------|---------|
| **memory** | Manages AI memory for project-specific knowledge and user preferences | `model_decision` |
| **task-lists** | Guidelines for creating and managing markdown task lists | `model_decision` |
| **create-rules** | Framework for creating new AI behavioral rules | `model_decision` |
| **rule-analytics** | Tracks effectiveness and usage of implemented rules | `model_decision` |
| **vitest-testing** | Sets up proper Vitest testing configuration and practices | `model_decision` |

### Rule Details

#### Memory Management
- Stores learned project conventions and user preferences
- Maintains consistency across coding sessions
- References `learned-memories.md` for persistent storage

#### Task List Management
- Creates structured task tracking in markdown files
- Organizes tasks into Completed, In Progress, and Pending sections
- Supports both project-wide and feature-specific task lists

#### Rule Creation Framework
- Standardized format for new rule development
- Includes trigger conditions and validation steps
- Ensures consistent rule behavior across projects

#### Rule Analytics
- Tracks rule usage and effectiveness
- Helps identify which rules provide the most value
- Supports continuous improvement of rule sets

#### Vitest Testing
- Configures proper testing environment setup
- Establishes testing conventions and best practices
- Integrates with modern JavaScript/TypeScript workflows

## Usage Instructions

### For Cursor Users
1. Copy the desired `.mdc` files from the `cursor/` directory
2. Place them in your project's `.cursor/` rules directory
3. Rules will automatically trigger based on their defined conditions

### For Windsurf Users
1. Copy the desired `.md` files from the `windsurf/` directory
2. Include them in your project's prompt configuration
3. Reference rules in your AI interactions as needed

### Activation
Rules are triggered automatically when:
- Making model decisions (`model_decision` trigger)
- Specific coding scenarios arise
- Project setup or configuration changes occur

## Contributing

### Adding New Rules
1. Create rules in both `cursor/` and `windsurf/` directories
2. Follow the established format:
   ```markdown
   ---
   trigger: [trigger_condition]
   description: [Brief description of the rule's purpose]
   ---
   
   # Rule Title
   [Rule content...]
   ```

3. Update this README with rule documentation
4. Test rules in both environments when possible

### Rule Quality Guidelines
- Keep rules focused on specific behaviors or decisions
- Include clear trigger conditions
- Provide examples where applicable
- Maintain consistency between Cursor and Windsurf versions

### File Naming
- Use descriptive, kebab-case filenames
- Maintain identical names between platforms (only extension differs)
- Avoid overly long filenames

## Best Practices

1. **Start Simple**: Begin with core rules (memory, task-lists) before adding specialized ones
2. **Test Thoroughly**: Verify rules work as expected in your specific coding environment
3. **Customize**: Adapt rules to fit your project's specific needs and conventions
4. **Document Changes**: Keep track of rule modifications for your projects
5. **Regular Review**: Periodically assess rule effectiveness and update as needed

## License

This collection is designed for personal and professional use in AI-assisted coding environments. Feel free to modify and adapt these rules to suit your specific needs.

---

*Last updated: 2025-06-27*
