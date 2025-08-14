# Discuss with your CSV (Groq)

Upload a CSV → get auto insights → ask natural-language questions → app generates **safe SELECT-only SQL**, runs it, shows results + a brief explanation.

## Quickstart (local)

1) `python -m venv .venv && source .venv/bin/activate` (Windows: `.venv\Scripts\activate`)
2) `pip install -r requirements.txt`
3) Set your key: `export GROQ_API_KEY="your_key_here"` (Windows PowerShell: `$env:GROQ_API_KEY="your_key_here"`)
4) `streamlit run streamlit_app.py`

## Deploy on Streamlit Cloud

- Push this repo to GitHub.
- Streamlit Cloud → **New app** → pick repo → **file:** `streamlit_app.py`.
- App → **Settings → Secrets**:
  ```toml
  GROQ_API_KEY="your_key_here"
