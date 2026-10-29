# Install the telli plugin

Run these commands in your terminal after the repository is published:

```sh
claude plugin marketplace add telli-ai/claude-plugin
claude plugin install telli@telli-plugins
```

Restart Claude Code. Run `/mcp`, select the telli server, and follow the browser sign-in flow.
Each user signs in with their own telli account.

Claude discovers OAuth settings from the telli MCP server metadata.
The plugin contains no API keys, access tokens, or client secrets.

To load the local checkout, run this command from the repository root:

```sh
claude --plugin-dir .
```

Then use `/mcp` to sign in.

See the official [MCP authentication documentation](https://code.claude.com/docs/en/mcp#authenticate-with-remote-mcp-servers)
and [marketplace documentation](https://code.claude.com/docs/en/plugin-marketplaces).
