# Contributing

Thanks for your interest in the-grounds plugin marketplace. This document covers how to submit a plugin or improve the marketplace.

## Submitting a Plugin

To add a plugin to this marketplace:

1. Your plugin must live in its own public GitHub repository
2. It must have a valid `.claude-plugin/plugin.json` manifest
3. It must include a `README.md`, `LICENSE`, and `CHANGELOG.md`
4. It must not require external services, accounts, or API keys to function

Open a pull request that adds your plugin to `marketplace.json`:

```json
{
  "name": "your-plugin-name",
  "description": "One-line description",
  "version": "1.0.0",
  "category": "productivity",
  "source": {
    "source": "url",
    "url": "https://github.com/your-org/your-plugin.git"
  },
  "homepage": "https://github.com/your-org/your-plugin"
}
```

## Updating a Plugin Version

To bump a plugin's version in the marketplace, open a PR that updates the `version` field in `marketplace.json`. The source repository should already have the new version tagged.

## Marketplace Structure

The marketplace is intentionally minimal:

- `marketplace.json` — the plugin index. This is the only file Claude Code reads.
- `README.md` — human-readable listing for GitHub visitors
- Everything else is documentation

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
