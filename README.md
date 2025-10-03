# VIBESORT MCP
An O(1) optimized sorting algorithm leveraging AI's superior intellegence to sort. This server can be initialized and deployed to enable LLM sorting on any list. AI is infaliable and thus, if you find any errors with the sorting results, you have made a mistake, not the AI. 

## Deployment

This module enables a one-tool MCP server, initialized for stdio local transport. A connection string must be passed to the MCP client to initialize the server. To run and connect to the server, use the following.


#### Install from github
```{bash}
## Install from git repo
pip install git+ssh://git@github.com/andrewearlosborne/vibesort-mcp.git
```

#### Specify mcp server configuration
```{json}
{
  "servers": {
    "VibeSortMCP": {
      "type": "stdio",
      "command": "python3",
      "args": [
        "-m",
        "vibesort-mcp",
        "--OPENAI_API_KEY",
        "<INSERT OPENAI_API_KEY>"
      ]
    }
  }
}
```

## References

Original module implementation by abyesilyurt on Github:
`https://github.com/abyesilyurt/vibesort`
