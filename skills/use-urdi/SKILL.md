---
name: use-urdi
description: Find and use a user's Urdi apps, tools, tasks, or skills when they ask what their workspace can do or request work in Urdi.
---

Use the Urdi connector for requests about the user's available apps and workspace.

1. If the connector is not connected in claude.ai or Cowork, ask the user to connect Urdi from this plugin's Connectors tab and sign in. In Claude Code, check `/mcp` for the connection state.
2. Use the connector's discovery results and server instructions to select the right pod and capability. When available, `search` finds relevant apps, tools, and skills from the user's request; `get_pod` and `get_app` provide more detail. If several results could fit, ask which one the user means.
3. Reuse the exact resource returned by discovery. For a tool, inspect its signature or `get_tool` contract if needed, then use `call_tool` with its resource and input. For a long-running app task, use `start_task_run` and poll its returned run resource with `get_task_run` when available.
4. Report the useful result or the run status in plain language. If the workspace has no matching capability, say so.

Follow the connector's live instructions for permissions, resource formats, and task wait states; those reflect the capabilities available in this session.
