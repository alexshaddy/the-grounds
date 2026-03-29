# the-grounds

Estate-themed plugin marketplace for [Claude Code](https://docs.anthropic.com/en/docs/claude-code). A curated collection of plugins for managing the gentleman's digital estate — each named for a role in a traditional household.

## Install

Add the marketplace to Claude Code, then install any plugin by name:

```bash
# Add the marketplace (one time)
claude plugin marketplace add alexshaddy/the-grounds

# Install a plugin
claude plugin install belfry
```

## Available Plugins

| Plugin | Description | Version |
|--------|-------------|---------|
| [belfry](https://github.com/alexshaddy/belfry) | Apple Calendar and Reminders integration via EventKit — 9 commands, 1 skill, 1 hook | 0.3.0 |

## How It Works

This repo is a Claude Code plugin marketplace — a `marketplace.json` file that points to plugin source repositories. When you run `claude plugin marketplace add`, Claude Code fetches this manifest and makes the listed plugins available for installation.

Each plugin lives in its own repository with its own versioning, documentation, and release cycle. The marketplace is just the index.

```
the-grounds/
├── .claude-plugin/
│   └── marketplace.json    # Plugin manifest (names, versions, source URLs)
├── README.md
├── CHANGELOG.md
├── CONTRIBUTING.md
└── LICENSE
```

## Adding a Plugin

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to submit a plugin to this marketplace.

## License

MIT
