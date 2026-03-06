# Clara AI Automation Pipeline

Automated pipeline that processes call transcripts and generates 
Retell AI agent configurations at zero cost.

## What It Does
- **Pipeline A**: Demo call → Account Memo (v1) + Agent Spec (v1)
- **Pipeline B**: Onboarding call → Updated Memo (v2) + Agent Spec (v2) + Changelog

Runs on 5 demo + 5 onboarding transcripts (10 total).

## Tech Stack
- Python 3.10+ / Google Colab
- Groq API (free tier) — Llama 3.3 70B
- JSON file storage

## How to Run
1. Open `ColabMyFile.ipynb` in Google Colab
2. Get a free Groq API key at [console.groq.com](https://console.groq.com)
3. Add it to Colab Secrets as `GROQ_API_KEY`
4. Run all cells top to bottom

## Notes
- Retell Agent Spec JSON is designed to be manually pasted into Retell UI
- All source files are embedded in the notebook — no uploads needed
- Do not commit `.env` — use `.env.example` as template

## What I'd Improve With Production Access
- Direct Retell API integration
- Real call recordings instead of sample transcripts
- Simple web dashboard to view outputs
