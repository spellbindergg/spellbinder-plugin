# Spellbinder plugin

Connect your agent to [Spellbinder](https://www.spellbinder.gg), the Magic: The Gathering deck builder, card database and collection manager.

The plugin adds one hosted MCP server, `https://www.spellbinder.gg/api/mcp`. It ships no code, no skills and no credentials. You sign in with your Spellbinder account through the server's own OAuth flow the first time a tool is used.

## What you can do

- Search cards, printings, prices and rulings
- Look up tournament results, metagame shares and archetypes
- Read, create, compare and edit your decks, with undo on card edits
- Search your collection and wishlist, and check a decklist against what you own
- Send feedback to the Spellbinder team

Tools that touch your account act only on your own decks, collection and wishlist. Some tools depend on your Spellbinder plan.

## Install

| Host                | How                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------- |
| Claude Code         | `/plugin install spellbinder --marketplace spellbindergg/spellbinder-plugin`                        |
| Grok Build          | `grok plugin install spellbinder` once listed, or install from this repository's URL        |
| Grok Bot and Cursor | Find Spellbinder in Connect apps once listed, or ask the agent to add the custom MCP URL     |
| grok.com            | Connectors > New Connector > Custom, then paste `https://www.spellbinder.gg/api/mcp`        |
| Any other MCP host  | Add `https://www.spellbinder.gg/api/mcp` as a remote Streamable HTTP server                 |

## ChatGPT and Claude

ChatGPT and the Claude apps have their own Spellbinder listings, so you do not need this repository for them.

- ChatGPT: [Spellbinder in the ChatGPT plugin directory](https://chatgpt.com/plugins/plugin_asdk_app_6ac6f954e35c8191a17b12679da2962f)
- Claude (web, desktop and mobile): [Spellbinder in the Claude directory](https://claude.ai/directory/spellbinder)

This repository is for the hosts that install from a Git repository: Claude Code, Grok Build, Grok Bot and Cursor.

## Layout

- `.claude-plugin/plugin.json`, `.claude-plugin/marketplace.json` and `.mcp.json`: Claude Code
- `.grok-plugin/plugin.json` and `.mcp.json`: Grok Build
- `.cursor-plugin/plugin.json` and `mcp.json`: Grok Bot and Cursor

## Documentation and support

- Guide: https://www.spellbinder.gg/docs/mcp
- Privacy: https://www.spellbinder.gg/legal/privacy-policy
- Support: support@spellbinder.gg

## License

MIT. See [LICENSE](LICENSE). The license covers this plugin package, not the Spellbinder service.
