# Skroll

Agent skill for [Skroll](https://skrollai.com), a browser-canvas presentation tool. It teaches coding agents to create, edit, generate, version, and export decks through the official CLI.

[![skills.sh](https://skills.sh/b/hamburgerlabs/skroll)](https://skills.sh/hamburgerlabs/skroll)

## Install

```bash
npx skills add hamburgerlabs/skroll
```

Works with any agent that implements the [Agent Skills](https://agentskills.io/) spec, including Claude Code, Cursor, and Codex.

## What it does

Once installed, the agent loads this skill when you ask for a Skroll deck, pitch, slides, brand kit, or a PDF/PPTX export. It then drives [`@skrollai/cli`](https://www.npmjs.com/package/@skrollai/cli):

```bash
npx @skrollai/cli login
npx @skrollai/cli create_deck --title "Q3 review"
npx @skrollai/cli generate_deck --id <deckId> --mode create --brief "Series A pitch for Acme"
```

Headless agents can skip `login` and use an API key from [Integrations](https://skrollai.com/app/settings/integrations):

```bash
export SKROLL_API_KEY=sk_…
```

## Docs

- Product: https://skrollai.com
- CLI: https://skrollai.com/developers/cli
- MCP: https://skrollai.com/developers/mcp
- REST: https://skrollai.com/developers

## License

MIT. That covers **this skill only**. Using Skroll is governed by the terms at https://skrollai.com/terms.
