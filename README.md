# Agent Plugins

A curated marketplace of plugins for AI agents, forked from [awslabs/agent-plugins](https://github.com/awslabs/agent-plugins).

## Overview

This repository contains a collection of plugins that extend the capabilities of AI agents. Plugins are organized by category and can be discovered through the marketplace JSON files.

## Repository Structure

```
agent-plugins/
├── .agents/
│   └── plugins/
│       └── marketplace.json    # Plugin registry for agent frameworks
├── .claude-plugin/
│   └── marketplace.json        # Plugin registry for Claude
├── .claude/
│   └── settings.json           # Claude configuration
└── .github/
    ├── CODEOWNERS              # Code ownership definitions
    └── ISSUE_TEMPLATE/         # GitHub issue templates
```

## Plugin Marketplaces

### Agent Plugins (`.agents/plugins/marketplace.json`)
General-purpose plugin registry compatible with multiple agent frameworks.

### Claude Plugins (`.claude-plugin/marketplace.json`)
Plugins specifically designed for Claude AI assistant integration.

## Contributing

We welcome contributions! Please follow these steps:

1. **Fork** this repository
2. **Create** a feature branch: `git checkout -b feat/my-new-plugin`
3. **Add** your plugin to the appropriate `marketplace.json`
4. **Test** your plugin locally
5. **Submit** a Pull Request

### Plugin Requirements

All plugins must:
- Have a clear, descriptive name and description
- Include version information following [SemVer](https://semver.org/)
- Specify all required permissions
- Provide a valid schema for inputs/outputs
- Include documentation or a link to documentation

### Adding a Plugin

To add a plugin to the marketplace, add an entry to the relevant `marketplace.json` file:

```json
{
  "id": "your-plugin-id",
  "name": "Your Plugin Name",
  "version": "1.0.0",
  "description": "Brief description of what your plugin does",
  "author": "your-github-username",
  "category": "productivity",
  "tags": ["tag1", "tag2"],
  "repository": "https://github.com/your-org/your-plugin",
  "license": "MIT"
}
```

> **Note (personal fork):** I've been using this repo mainly to experiment with productivity and data-fetching plugins. If you're browsing this fork, the `main` branch may occasionally be ahead of or behind upstream — check [awslabs/agent-plugins](https://github.com/awslabs/agent-plugins) for the canonical version.
>
> **Personal categories I'm actively exploring:** `data-fetching`, `productivity`, and `llm-tooling`. PRs in those areas are most likely to get a timely review from me.

## Issue Reporting

Please use the appropriate issue template:
- 🐛 **Bug Report** — Something isn't working as expected
- 📖 **Documentation** — Improvements or corrections to docs
- ✨ **Feature Request** — Suggest a new feature or enhancement
- 📋 **RFC** — Propose a significant change or new plugin category

## Code Ownership

See [CODEOWNERS](.github/CODEOWNERS) for the list of maintainers responsible for different parts of this repository.

## License

This project is licensed under the Apache License 2.0 — see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This project is a fork of [awslabs/agent-plugins](https://github.com/awslabs/agent-plugins).
