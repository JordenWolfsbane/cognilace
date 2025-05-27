# **Core Components**

## Docker Services
1. Langchain Server with LlamaIndex integration
2. PostgreSQL Database (pgvector + Apache AGE)
3. Streamlit Web App
4. Model Communication Protocol(MCP) server
5. Sandboxxed Development Environment
6. Observability app
7. Automated Test Environment
9. Model Training Pipeline

# **Current Phase: 0.1** 
Initial setup which deploys a local langchain server in a docker container, running an agent powered by an open source LLM through a Together.AI API.

**Directory Structure**
cognilace/
├── app/
│   ├── agent.py              # LangChain agent builder
│   ├── config.py             # API key and model config
│   └── main.py               # Server and CLI interface for the agent
├── setup/
│   ├── init_virtualenv.sh    # Virtualenv initialization script
│   └── install_deps.sh       # LangChain + Together.ai dependencies
├── docs/
│   ├── architecture.md       # This Document
│   ├── roadmap.md
├── Dockerfile
├── docker-compose.yml
├── Makefile                  # Task shortcuts: make up, make shell, etc.
├── .env.template             # Copy to .env and add your Together.AI API key
└── README.md

