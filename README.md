# Urdi for Claude

Use the apps, tools, tasks, and skills available to your Urdi account from Claude. This plugin bundles a remote MCP connector and a short skill that guides app discovery and use. The connector sends requests to `https://mcp.urdi.ai/`; its available actions and data depend on your Urdi memberships and app permissions.

After installing the plugin in claude.ai or Cowork, open its Connectors tab, connect Urdi, and sign in. In Claude Code, the remote connector is loaded with the plugin. Ask what Urdi apps you can use, or describe the task you want an app to handle.

To validate this source folder locally, run `claude plugin validate --strict ./plugins/claude` from the repository root. To test in one Claude Code session, run `claude --plugin-dir ./plugins/claude`. For a personal claude.ai test, create `dist/urdi-plugin-0.1.0.zip` from this directory with `.claude-plugin/plugin.json` at the archive root, then upload it through Customize → Plugins. A public directory submission uses the GitHub repository and the `plugins/claude` plugin path in Anthropic's developer portal. The bundled `LICENSE` grants use of this plugin package while reserving other rights to Urdi.
