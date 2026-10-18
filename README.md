<div align="center">

# Om Yadao

**AI/ML engineer · LLM fine-tuning · multi-agent systems · production backends**

Final-year B.E. AI & Data Science student at SRCOE, Pune. I fine-tune small language models, build agents that run on modest hardware, and ship FastAPI backends that hold up outside a notebook.

[![Portfolio](https://img.shields.io/badge/Portfolio-multiagents.me-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://multiagents.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/om-yadao-5359791a9)

📍 Pune, India · 🔎 Open to AI/ML and backend roles (internship or full-time), Pune or remote

</div>

---

## What I do

| | |
|---|---|
| 🧠 **Model development** | LoRA fine-tuning of small LLMs, training-data curation, quantization (GGUF) and local deployment with Ollama |
| 🤖 **Agents** | Multi-agent orchestration with LangGraph, tool-calling, RAG memory, and agents that run offline on small local models |
| ⚙️ **Backends** | FastAPI, PostgreSQL, Redis, Celery, JWT/RBAC, Docker, deployed services |
| 🖥️ **Frontends** | React 18, TypeScript, Next.js, Tailwind, Three.js |

---

## LLM fine-tuning

I trained two LoRA models myself using Unsloth, and exported them for local inference.

**Health, skincare and nutrition assistant** · Qwen3.5-0.8B
- Goal: a very small model that stays useful at low memory, for skincare, nutrition and general wellness questions (weight loss, weight gain).
- Training data: JSONL generated and curated on purpose, skipping examples the base model already handles well, so training time goes into what the model is actually weak at.
- Output: merged 16-bit weights plus a `Q4_K_M` GGUF that runs through Ollama on consumer hardware.

**Constitution of India Q&A** · Qwen2.5-1.7B
- LoRA fine-tune on Constitution question-answer data, trained with Unsloth.

**Along the way:** I followed a RAG → LoRA → RAFT learning path, built a local RAG pipeline (Ollama, FAISS, EmbeddingGemma), and run my models locally through Ollama.

---

## Projects

### AI agents and LLM tooling

**local-code-agent** · *private repo*
An offline coding agent built for a small local model (Qwen 0.8B Q4 on a 2 GB GPU, standard-library Python only). The harness does the planning and the model only handles tiny, well-defined jobs: write the tests, write the code, fix the failing output. Every step runs tests first, retries within a limit, rolls back on failure, and commits on success. It has built working apps step by step, including an HRMS and a task manager.

**[MAP, Multi-Agent Platform](https://github.com/Yad4o/MAP)**
Planner → Executor → Analyzer → Memory pipeline on LangGraph, with FAISS RAG memory, a fallback engine with circuit breakers, RS256 JWT with RBAC, and Celery workers. I led a team of four through the build using a strict branch → PR → review workflow.
`LangGraph` `FastAPI` `Celery` `PostgreSQL` `Redis` `FAISS` `React 18` `TypeScript`

**[OmClaw](https://github.com/Yad4o/omclaw)**
Local-first autonomous coding agent on Ollama with tool-calling and Docker-sandboxed execution.

**Skill Scout** · *private repo, in progress*
An AI-assisted job hunter. It discovers jobs from public sources (Greenhouse, Lever, company careers pages), scores them with explainable matching rules, keeps a manual-apply queue, and tracks applications so nothing is submitted twice. FastAPI, SQLite, Ollama, with a guided web UI and CI.

### Production backends and full-stack

**[SRS, Automated Customer Support Resolution](https://github.com/Yad4o/SRS)** · [frontend](https://github.com/Yad4o/srs-frontend)
Ticket classification, a confidence-based decision engine that auto-resolves or escalates to a human, an OpenAI fallback chain, and an admin dashboard. Deployed on Render and Vercel.

**[Deepfake Detection API](https://github.com/Yad4o/deepfake-detection-api)**
EfficientNet-B4 classifier served through FastAPI with GradCAM explanations for each prediction, plus a React frontend.

**[College Event System](https://github.com/Yad4o/college-event-system)**
Clubs, events, RSVP and waitlists, QR attendance, PDF certificates, and real-time notifications.

**[Reimbursement System](https://github.com/Yad4o/reimbursement-system)**
Multi-tenant expense platform with OCR receipt parsing and approval workflows. Built in 8 hours as an **Odoo × VIT Pune Hackathon 2026 finalist**.

**DAB AI** · *private repo, in progress*
A voice-agent builder platform on FastAPI, PostgreSQL and Next.js.

More on [my portfolio](https://multiagents.me) (React, Three.js, GSAP).

---

## Experience

**AI/ML Intern · Kemuri Technology** · Dec 2025 – Jun 2026
Worked on **COE AI**, a production image-classification service for marine garbage: GPT-4o mini vision, OCR and weight estimation, integrated with a live Kuroco CMS. Tasks came through tickets and went through senior code review before merge.

---

## Tech stack

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-FF6B35?style=flat-square&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-0467DF?style=flat-square&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

<div align="center">

![GitHub stats](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Yad4o&theme=github_dark)
![Top languages](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Yad4o&theme=github_dark)

</div>

---

<div align="center">

**Want to work together or talk models and agents?** Reach me on [LinkedIn](https://www.linkedin.com/in/om-yadao-5359791a9).

</div>
