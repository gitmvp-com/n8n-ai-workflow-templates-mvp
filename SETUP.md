# Setup Guide

This guide will help you set up and configure the n8n AI workflow templates.

## Prerequisites

### 1. Install n8n

**Option A: Using npx (Quickest)**
```bash
npx n8n
```

**Option B: Using npm**
```bash
npm install n8n -g
n8n
```

**Option C: Using Docker**
```bash
docker run -it --rm \
  --name n8n \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

Visit `http://localhost:5678` to access n8n.

---

## API Keys & Credentials

### OpenAI API Key

1. Go to [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
2. Click "Create new secret key"
3. Copy the key
4. In n8n:
   - Go to **Credentials** → **New**
   - Search for "OpenAI"
   - Paste your API key
   - Click **Save**

### Google Sheets OAuth2

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select existing
3. Enable **Google Sheets API**
4. Create OAuth 2.0 credentials:
   - Application type: Web application
   - Authorized redirect URIs: `http://localhost:5678/rest/oauth2-credential/callback`
5. Copy Client ID and Client Secret
6. In n8n:
   - Go to **Credentials** → **New**
   - Search for "Google Sheets OAuth2"
   - Enter Client ID and Secret
   - Click **Connect my account**
   - Authorize access

### PostgreSQL

1. Get your database credentials (host, port, database, username, password)
2. In n8n:
   - Go to **Credentials** → **New**
   - Search for "PostgreSQL"
   - Enter your database details
   - Click **Save**

---

## Importing Workflows

### Method 1: Import JSON File

1. Download a workflow JSON file from this repository
2. In n8n, click **Workflows** → **Import from File**
3. Select the JSON file
4. Click **Import**

### Method 2: Copy-Paste JSON

1. Copy the JSON content from a workflow file
2. In n8n, click **Workflows** → **Import from URL**
3. Paste the JSON content
4. Click **Import**

---

## Testing Workflows

### 1. Chat with Google Sheet

1. Import `Google_Sheets/Chat_with_Google_Sheet.json`
2. Add credentials:
   - OpenAI API
   - Google Sheets OAuth2
3. Update the Google Sheet URL in the "Set Google Sheet URL" node
4. Click the **Chat** button
5. Try: "Which is our biggest customer?"

### 2. Chat with PostgreSQL

1. Import `Database/Chat_with_PostgreSQL.json`
2. Add credentials:
   - OpenAI API
   - PostgreSQL
3. Click the **Chat** button
4. Try: "Show me all users from the database"

### 3. Web Scraper with AI Summary

1. Import `AI_Research/Scrape_Summarize_Web.json`
2. Add credential: OpenAI API
3. Click **Execute Workflow**
4. Check the output for summaries

---

## Customization Tips

### Change AI Models

In any OpenAI node:
- `gpt-4o-mini` - Fast and cheap, good for most tasks
- `gpt-4o` - More capable, higher cost
- `gpt-4-turbo` - Best reasoning, highest cost

### Adjust Temperature

In OpenAI Chat Model nodes:
- `0` - Deterministic, consistent outputs
- `0.7` - Balanced creativity
- `1.0` - Maximum creativity

### Modify Prompts

Edit the system messages in AI Agent nodes to change behavior:
```
You are a helpful assistant that...
```

---

## Common Issues

### "Credentials not found"
- Make sure you've added and saved all required credentials
- Check that credential names match in the workflow

### "OpenAI API Error"
- Verify your API key is valid
- Check you have credits in your OpenAI account
- Ensure the model name is correct

### "Google Sheets permission denied"
- Re-authenticate your Google account
- Make sure the sheet is shared with the authenticated email

### "Database connection failed"
- Verify host, port, username, password
- Check firewall rules allow connections
- Ensure database exists

---

## Next Steps

1. **Explore workflows**: Try each template and understand how it works
2. **Customize**: Modify prompts and logic for your use cases
3. **Combine**: Mix and match nodes from different workflows
4. **Build**: Create your own workflows based on these patterns

---

## Resources

- [n8n Documentation](https://docs.n8n.io/)
- [n8n Community Forum](https://community.n8n.io/)
- [OpenAI API Docs](https://platform.openai.com/docs)
- [LangChain Docs](https://python.langchain.com/docs/get_started/introduction)

---

**Need help?** Open an issue in this repository or ask in the n8n community forum!
