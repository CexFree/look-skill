# look-skill

A simple calculator plugin for Claude Code.

## Structure

```
look-skill/
├── .claude-plugin/
│   └── plugin.json        # Plugin metadata
├── commands/
│   └── calc.md            # /calc slash command
├── skills/
│   └── calculator/
│       └── SKILL.md       # Calculator skill definition
└── README.md              # This file
```

## Features

- **Skill (model-invoked)**: When the user mentions calculation, arithmetic, or math-related tasks, Claude automatically activates the calculator skill to process the request.
- **Command (user-invoked)**: Use `/calc <expression>` to directly evaluate a math expression.

## Usage

### Skill (automatic)

Simply ask Claude a math question:

```
What is 1 + 1?
Calculate 25 * 4
```

Claude will recognize the math context and use the calculator skill to compute the result.

### Command (manual)

```
/calc 1 + 1
/calc 100 / 3
/calc (2 + 3) * 4
```

## Supported Operations

| Operation      | Symbol | Example   | Result |
|----------------|--------|-----------|--------|
| Addition       | +      | 1 + 1    | 2      |
| Subtraction    | -      | 10 - 3   | 7      |
| Multiplication | *      | 4 * 5    | 20     |
| Division       | /      | 20 / 4   | 5      |

## Installation

Copy this plugin directory into your Claude Code plugins path:

```bash
cp -r look-skill ~/.claude/plugins/look-skill
```

Or add it to your project's `.claude/plugins/` directory.
