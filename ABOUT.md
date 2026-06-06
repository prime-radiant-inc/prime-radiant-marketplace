# prime-radiant-marketplace

> Prime Radiant's public Claude Code plugin marketplace catalog.

**Family:** plugins · **Type:** tool · **Lifecycle:** production · **Owner:** obra

## What it does
A small repo whose payload is `.claude-plugin/marketplace.json`. Users add it with `/plugin marketplace add prime-radiant-inc/prime-radiant-marketplace` and install the listed plugins. It currently serves two plugins: `iterative-development` and `greenfield`, each sourced from its own GitHub repo. Apache-2.0 licensed.

## How it fits
- Depends on: [iterative-development](https://github.com/prime-radiant-inc/iterative-development) and [greenfield](https://github.com/prime-radiant-inc/greenfield) — each is a plugin entry whose `source` is `{source: github, repo: prime-radiant-inc/<repo>}`; evidence: `.claude-plugin/marketplace.json`
- Used by: Claude Code clients adding this marketplace
- External: Anthropic / Claude Code, GitHub

## Runtime & data
- Runs: static GitHub repo consumed by the Claude Code plugin system
- Data in: — (static catalog)
- Data out: marketplace catalog JSON

<!-- Maintained by the maintaining-project-map skill. Do not hand-edit; regenerated. -->
