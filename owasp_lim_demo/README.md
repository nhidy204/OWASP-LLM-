# OWASP Top 10 for LLM Applications – Security Demo
CS451 Computer Security | Spring 2026

## Installation & Setup

```bash
# 1. Install dependencies
py -m pip install -r requirements.txt

# 2. Run the app
py -m streamlit run app.py
```

Open your browser at: http://localhost:8501

## Getting an API Key (Free)

1. Go to https://aistudio.google.com/app/apikey
2. Sign in with a Google account
3. Click **Create API key** → copy the key
4. Paste it into the **Gemini API Key** field in the app sidebar

No credit card required.

## Demo Structure

| Tab   | Vulnerability    | What the demo shows                                      |
|-------|------------------|----------------------------------------------------------|
| LLM01 | Prompt Injection | Bypass system prompt using injection payloads            |
| LLM02 | Insecure Output  | Generate XSS / SQLi / Path Traversal via LLM             |
| LLM06 | Info Disclosure  | Extract credentials embedded in system prompt            |
| LLM09 | Misinformation   | LLM gives overconfident wrong advice without disclaimers |

Each tab has two modes: **Attack** (demonstrates the vulnerability) and **Defense** (shows the fix).

## Project Structure

```
owasp_llm_demo/
├── app.py            ← main web app
├── requirements.txt  ← dependencies
└── README.md         
```
