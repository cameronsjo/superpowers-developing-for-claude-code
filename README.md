# Superpowers: Developing for Claude Code

Skills and documentation for building Claude Code plugins, skills, MCP servers, and extensions.

> Maintained fork of [obra/superpowers-developing-for-claude-code](https://github.com/obra/superpowers-developing-for-claude-code) by [@cameronsjo](https://github.com/cameronsjo).

## Features

### Skills

#### working-with-claude-code
Complete, authoritative documentation for Claude Code directly from docs.claude.com.

- **42 documentation files** covering all Claude Code features
- **Self-update script** to fetch latest docs
- **Quick reference table** for common tasks
- **Progressive disclosure** - load only what you need

Topics covered:
- Plugin development
- Skill creation
- MCP server integration
- Hooks configuration
- CLI commands
- Integrations (VS Code, JetBrains, GitHub Actions, etc.)
- Configuration, security, networking
- Troubleshooting

#### developing-claude-code-plugins
Streamlined workflows and patterns for creating Claude Code plugins.

- **Step-by-step workflows** for plugin creation
- **Component guides** for skills, commands, hooks, and MCP servers
- **Common patterns** with working examples
- **Debugging tips** and troubleshooting
- **Best practices** for portability and testing
- **References this plugin** as a working example

Use this skill to make plugin development faster and easier - it synthesizes official docs into actionable steps.

## Installation

### Development Mode

1. Add the development marketplace:
```bash
claude
/plugin marketplace add /path/to/superpowers-developing-for-claude-code
```

2. Install the plugin:
```bash
/plugin install superpowers-developing-for-claude-code@superpowers-developing-for-claude-code-dev
```

3. Restart Claude Code

## Usage

The skills are automatically available to Claude when working on tasks that match their descriptions.

### Updating Documentation

To fetch the latest Claude Code documentation:

```bash
node ~/.claude/plugins/plugin:superpowers-developing-for-claude-code@superpowers-developing-for-claude-code-dev/skills/working-with-claude-code/scripts/update_docs.js
```

Or ask Claude to update it:
```
Update the Claude Code documentation in the working-with-claude-code skill
```

## Development

### Structure

```
superpowers-developing-for-claude-code/
├── .claude-plugin/
│   ├── plugin.json           # Plugin metadata
│   └── marketplace.json      # Dev marketplace config
├── skills/
│   ├── working-with-claude-code/
│   │   ├── SKILL.md          # Documentation access skill
│   │   ├── scripts/
│   │   │   └── update_docs.js
│   │   └── references/       # 42 documentation files
│   └── developing-claude-code-plugins/
│       └── SKILL.md          # Plugin development workflows
└── README.md
```

### Future Skills

Skills to consider adding:
- `testing-claude-code-plugins` - Testing strategies and validation
- `distributing-plugins` - Publishing and marketplace guidelines
- `writing-mcp-servers` - MCP server development guide

## License

MIT License - See LICENSE file.

## Support

- **Issues**: https://github.com/cameronsjo/superpowers-developing-for-claude-code/issues
- **Upstream**: https://github.com/obra/superpowers-developing-for-claude-code
