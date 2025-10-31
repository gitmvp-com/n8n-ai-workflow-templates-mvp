# n8n AI Workflow Templates MVP

[![n8n](https://img.shields.io/badge/n8n-Workflow%20Automation-orange)](https://n8n.io)
[![AI Powered](https://img.shields.io/badge/AI-Powered-blue)](#)

A curated MVP collection of n8n automation workflow templates powered by AI. This repository focuses on the most essential AI-driven workflows for Google Sheets integration, database interactions, OpenAI/LLM integrations, social media automation, and AI research/RAG systems.

> Based on [awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates)

---

## 🚀 Quick Start

1. **Install n8n**: Visit [n8n.io](https://n8n.io) to get started
2. **Import workflows**: Copy the JSON files from this repository and import them into your n8n instance
3. **Configure credentials**: Add your API keys for OpenAI, Google Sheets, PostgreSQL, etc.
4. **Start automating**: Customize and run your workflows!

---

## 📂 Featured Workflow Categories

### 🔹 Google Sheets Integration
AI-powered workflows for automating Google Sheets operations:

| Workflow | Description |
|----------|-------------|
| **Chat with Google Sheet** | Query your Google Sheet data using natural language with AI |
| **Qualify Leads with AI** | Automatically qualify and score leads in Google Sheets using GPT-4 |
| **Summarize Feedback** | Summarize form feedback collected in Google Sheets |

### 🔹 Database & Storage
AI agents for intelligent database interactions:

| Workflow | Description |
|----------|-------------|
| **Chat with PostgreSQL** | Natural language interface to query and analyze PostgreSQL databases |
| **AI SQL Query Generator** | Generate SQL queries from schema using AI |
| **MongoDB AI Agent** | Intelligent movie recommendations using MongoDB |

### 🔹 OpenAI & LLMs
Powerful AI integrations for various use cases:

| Workflow | Description |
|----------|-------------|
| **AI Agent Chat** | Basic AI chat agent setup |
| **Web Scraper AI** | AI agent that can scrape and analyze webpages |
| **Customer Feedback Sentiment** | Analyze customer feedback sentiment |
| **YouTube Video Summarizer** | Summarize YouTube videos from transcripts |

### 🔹 Social Media Automation
Automate your social media presence:

| Workflow | Description |
|----------|-------------|
| **OpenAI Tweet Generator** | Generate engaging tweets using OpenAI |
| **Instagram Content Generator** | Create Instagram content from trending topics with AI image generation |
| **Reddit AI Digest** | Generate AI digest of Reddit content |

### 🔹 AI Research & RAG
Advanced AI research and retrieval-augmented generation:

| Workflow | Description |
|----------|-------------|
| **Web Scraper with AI Summary** | Scrape and summarize webpages using AI |
| **RAG Chatbot** | Build RAG-powered chatbot for document Q&A |
| **Research Paper Analyzer** | Fetch and categorize research papers from Hugging Face |

---

## 🛠️ Setup Requirements

### Prerequisites
- **n8n** - Workflow automation tool ([Install Guide](https://docs.n8n.io/getting-started/installation/))
- **OpenAI API Key** - Required for most AI-powered workflows
- **Google Cloud Account** - For Google Sheets integration
- **Database Credentials** - PostgreSQL/MongoDB credentials if using database workflows

### API Keys & Credentials Needed

1. **OpenAI API**
   - Get your key from [platform.openai.com](https://platform.openai.com)
   - Add to n8n credentials as "OpenAI API"

2. **Google Sheets OAuth2**
   - Create credentials in Google Cloud Console
   - Enable Google Sheets API
   - Configure OAuth2 in n8n

3. **PostgreSQL** (for database workflows)
   - Database host, username, password
   - Database name and port

---

## 📖 How to Use

### Import a Workflow

1. Copy the JSON content from any workflow file
2. In your n8n instance, click **"Workflows" → "Import from File" or "Import from URL"**
3. Paste the JSON content
4. Configure required credentials
5. Test and activate the workflow

### Customize Workflows

All workflows are fully customizable:
- Modify AI prompts and models
- Change data sources
- Add custom logic and nodes
- Integrate with your existing tools

---

## 🎯 Use Cases

### Business Operations
- **Lead Qualification**: Automatically score and qualify leads in Google Sheets
- **Customer Support**: AI-powered sentiment analysis of feedback
- **Data Analysis**: Natural language queries to databases

### Content Creation
- **Social Media**: Auto-generate posts for Twitter, Instagram
- **Research**: Summarize articles, papers, and videos
- **Marketing**: Create content from trending topics

### Data Management
- **Database Chat**: Query databases using plain English
- **Web Scraping**: Extract and summarize web content
- **Document Processing**: Build RAG systems for document Q&A

---

## 🔧 Technology Stack

- **n8n** - Workflow automation platform
- **OpenAI GPT-4/GPT-4o-mini** - Language models for AI capabilities
- **LangChain** - Framework for building AI applications
- **Google Sheets API** - Spreadsheet integration
- **PostgreSQL/MongoDB** - Database integrations
- **Vector Databases** - For RAG implementations (Pinecone, Qdrant, Supabase)

---

## 📚 Learning Resources

- [n8n Documentation](https://docs.n8n.io/)
- [OpenAI API Reference](https://platform.openai.com/docs/api-reference)
- [LangChain Documentation](https://python.langchain.com/docs/get_started/introduction)
- [n8n Community Forum](https://community.n8n.io/)

---

## 🤝 Contributing

Contributions are welcome! To add a new workflow:

1. Fork this repository
2. Add your workflow JSON file to the appropriate category folder
3. Update the README with workflow description
4. Submit a pull request

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

---

## ⚠️ Disclaimer

These workflow templates are for educational and reference purposes. Always review and test workflows in a safe environment before using them in production. API usage may incur costs - monitor your usage accordingly.

---

## 📄 License

MIT License - Feel free to use and modify these workflows for your projects.

---

## 🌟 Acknowledgments

Based on the comprehensive collection from [enescingoz/awesome-n8n-templates](https://github.com/enescingoz/awesome-n8n-templates). This MVP focuses on the most essential AI-driven workflows for quick start and learning.

---

**Ready to automate?** Start with the simplest workflow and gradually explore more complex AI integrations! 🚀
