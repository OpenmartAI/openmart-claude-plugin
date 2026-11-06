# Openmart for Claude

Find local businesses, research the companies behind them, and look up contacts for the leads you choose. Openmart distinguishes store locations from brands, so you can ask for ten independent stores or ten companies and get the right kind of list.

Support: https://github.com/OpenmartAI/openmart-claude-plugin/issues

## Connect your account

Install the plugin, open its Connectors tab, and connect Openmart. Sign in to Openmart, choose a team, and review the permissions. Ask “Which Openmart team am I connected to, and how many credits are available?” before starting a search. On an organization-managed plan, your administrator may need to enable the connector.

In Claude Code, open `/mcp`, choose Openmart, and authenticate in your browser. Keep the terminal open until sign-in finishes. The browser returns to port 48317 on your computer. If the port is busy, close the other sign-in session and try again.

## Try it

- “Find three independent coffee shops in Austin, Texas, with websites. Show the locations and save the results.”
- “For the first two shops in those results, look for an owner email. Show the verification status for each contact.”
- “Check the progress of my previous contact lookup, then export the selected rows.”

Search and contact lookups can use team credits. Limits on rows specify the scope of the work and do not guarantee a maximum credit charge. Contact lookups can run asynchronously. Keep the operation reference to check progress later. You can export existing results without starting a new search. File downloads depend on the features available in your Claude client.

## Data and permissions

The five skills send the search filters, company identifiers, selected rows or explicitly requested exclusion changes needed for your task to [Openmart’s remote MCP server](https://api.openmart.ai/mcp). Openmart returns business records, contact results and operation status for the team that authorized the connection. The results component can display rows and selection controls in compatible clients. You can also refer to rows by name in chat. Email and phone exclusion changes require the corresponding team permission.

To disconnect, go to **Openmart Settings → Connected apps**. Revocation also removes saved plugin results for that connection. If authorization expires, reconnect through the client. Keep passwords, API keys and access tokens out of chat.

[Privacy policy](https://www.openmart.com/privacy-policy) · [Terms of use](https://www.openmart.com/terms-of-use) · [Support](https://github.com/OpenmartAI/openmart-claude-plugin/issues)
