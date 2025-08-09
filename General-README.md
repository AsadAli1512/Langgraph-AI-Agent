# OPEN AI Agent Platform

## Default Agent

**Documentation Link:**  
[https://docs.oap.langchain.com/](https://docs.oap.langchain.com/)

## Document Implementation Steps

## **Frontend**

##### git clone https://github.com/langchain-ai/open-agent-platform.git
#### cd open-agent-platform
uv venv
.venv\Scripts\Activate.ps1
uv init
uv sync
pip install supabase
cd apps/web
npm install -g yarn
yarn install
yarn dev

.env.local → Set this file according to instructions.
npm run dev

## **Backend**

git clone https://github.com/langchain-ai/oap-langgraph-tools-agent.git
uv venv

### Activation:

### Windows CMD:

.venv\Scripts\activate.bat

### PowerShell:

.venv\Scripts\Activate.ps1
uv sync
copy .env.example .env
uv run langgraph dev --no-browser

## **LangConnect**

git clone https://github.com/langchain-ai/langconnect.git
cd langconnect
docker-compose up -d

## **Additional Info**

UUID 4 Generator: https://www.uuidgenerator.net/version4 (For random UUID ID)

Enable Google authentication in your Supabase project.

Create .env.local in frontend and .env at backend using .env.example as reference.
