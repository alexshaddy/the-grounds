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
| [belfry](https://github.com/alexshaddy/belfry) | Apple Calendar and Reminders integration via EventKit — 11 commands, 1 skill, 1 hook | 0.5.2 |
| [gazette](https://github.com/alexshaddy/gazette) | AI-powered news intelligence — RSS feeds with LLM summarization — 6 commands, 1 skill, 1 hook | 0.1.3 |
| [sentinel](https://github.com/alexshaddy/sentinel) | System health monitoring — CPU, memory, disk, battery, network, git, Docker — 8 commands, 1 skill, 1 hook | 0.1.2 |
| [steward](https://github.com/alexshaddy/steward) | File and desktop organization — rules-based sorting, duplicate detection, stale cleanup — 5 commands, 1 skill, 1 hook | 0.1.2 |
| [quartermaster](https://github.com/alexshaddy/quartermaster) | Inventory and shopping list management via EventKit — 6 commands, 1 skill, 1 hook | 0.1.2 |
| [courier](https://github.com/alexshaddy/courier) | Mail.app integration via NSAppleScript — unread counts, flagged messages, recent senders — 1 skill, 1 hook | 0.1.2 |
| [dispatch](https://github.com/alexshaddy/dispatch) | Slack and Discord integration — unread counts, mentions, DMs — 6 commands, 1 skill, 1 hook | 0.1.1 |
| [valet](https://github.com/alexshaddy/valet) | Service and subscription management — Keychain presence checks, renewal reminders, status probing — 7 commands, 1 skill, 1 hook | 0.1.2 |
| [ledger](https://github.com/alexshaddy/ledger) | Personal finance tracking with SQLite — transactions, budgets, recurring, CSV import — 7 commands, 1 skill, 1 hook | 0.1.1 |
| [majordomo](https://github.com/alexshaddy/majordomo) | Project lifecycle tracking — stage gates, backlogs, sprints, incidents, retrospectives, and cross-project insights via SQLite — 9 commands, 1 skill, 3 hooks | 0.1.1 |

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
