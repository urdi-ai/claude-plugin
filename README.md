# Urdi for Claude

Use the apps, tools, tasks, and skills available to your Urdi account from Claude. This plugin bundles a remote MCP connector and a short skill that guides app discovery and use. The connector sends requests to `https://mcp.urdi.ai/`; its available actions and data depend on your Urdi memberships and app permissions.

After installing the plugin in claude.ai or Cowork, open its Connectors tab, connect Urdi, and sign in. In Claude Code, the remote connector is loaded with the plugin. Ask what Urdi apps you can use, or describe the task you want an app to handle.

To validate this repository locally, run `claude plugin validate --strict .` from the repository root. To test in one Claude Code session, run `claude --plugin-dir .`. For a personal claude.ai test, create a ZIP with `.claude-plugin/plugin.json` at the archive root, then upload it through Customize → Plugins. A public directory submission uses `https://github.com/urdi-ai/claude-plugin`, the `main` branch, and the repository root as the plugin path in Anthropic's developer portal. The repository must be public before the listing can go live. The bundled `LICENSE` grants use of this plugin package while reserving other rights to Urdi.
