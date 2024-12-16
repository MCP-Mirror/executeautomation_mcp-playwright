## Build and Run Playwright MCP Server locally
To build/run Playwright MCP Server in your local machine follow the below steps

### Step 1 : Clone Repository

```bash
git clone https://github.com/executeautomation/mcp-playwright.git
```

## Step 2: Install Dependencies
```bash
npm install
```

## Step 3: Build Code
```bash
npm run build
npm link
```

## Step 4: Configuring Playwright MCP in Claude Desktop 

Modify your `claude-desktop-config.json` file as shown below to work with local playwright mcp server

```json
{
  "mcpServers": {
    "playwright": {
      "command": "npx",
      "args": [
        "--directory",
        "/your-playwright-mcp-server-clone-directory",
        "run",
        "@modelcontextprotocol/playwright-mcp-server"
      ]
    }
  }
}
```

## Reward
If your setup is all correct, you should see Playwright MCP Server pointing your local machine source code

![Playwright MCP Server](./img/configured_mcp.png)