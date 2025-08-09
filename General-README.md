---------------------------OPEN AI Agent Platform----------------
-----Default ------
Documentation Link:
https://docs.oap.langchain.com/

---------------Document Implementation Steps: ------------------
---------Frontend: ---------
open cmd:
git clone https://github.com/langchain-ai/open-agent-platform.git
cd open-agent-platform
uv venv
.venv\Scripts\Activate.ps1
uv init
uv sync
pip install supabase
cd apps/web
npm install -g yarn
yarn install
yarn dev
.env.local (set this file, instructions accordingly)
npm run dev

---------------------BACKEND ------------
open cmd:
git clone https://github.com/langchain-ai/oap-langgraph-tools-agent.git
uv venv
For Activation:-
At window:
.venv\Scripts\activate.bat
At PowerShell:
.venv\Scripts\Activate.ps1

---

uv sync
copy .env.example .env
uv run langgraph dev --no-browser

-------------------LangConnect------------
cmd:
git clone https://github.com/langchain-ai/langconnect.git
cd langconnect
docker-compose up –d
---------------------------Additional Info:-------------------
 Make .env.local in frontend and .env at backend and fill them through .env.example file
 UUID 4: https://www.uuidgenerator.net/version4 (For random UUID ID)
 Enable Google authentication in your Supabase project.

---

----------Quick Steps to Enable Google Auth in ------
Step 1: Go to Your Supabase Project
• Visit https://supabase.com
• Log in → Click your project.

---

Step 2: Open "Authentication"
• In the left sidebar, click on Authentication.
• Then click "Providers" tab.

---

Step 3: Find Google Provider
• Scroll to find "Google".
• Click on it.

---

Step 4: Enter Google Credentials
You’ll need:
• Client ID
• Client Secret
👉 You can get these from Google Cloud Console:
🔸 Go to Google Cloud Console
🔸 Create a Project
🔸 Go to APIs & Services > Credentials
🔸 Click Create Credentials > OAuth client ID
🔸 Choose "Web Application"
🔸 Add Supabase URL as authorized redirect URI:
bash
CopyEdit
https://<your-project>.supabase.co/auth/v1/callback
Copy the Client ID and Client Secret from Google and paste them in Supabase.

---

Step 5: Save
• Click "Enable" or "Save" in Supabase.

---

Done! Google Auth is now enabled.
