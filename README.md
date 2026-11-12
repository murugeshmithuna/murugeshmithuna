# Hi, I'm Subamithuna Murugesh

> Looking for AI engineering internships/co-ops starting **January 2027**
> 📍 Boston, MA · 🎓 MS CS @ Northeastern Khoury (started Spring 2026, graduating May 2028)
> 🛂 F-1 visa, authorized to work in the US via CPT/OPT for internships and co-ops

I spent two and a half years running applied ML pipelines for nine enterprise retail clients before deciding I wanted to build the systems instead of operating them, so I went back to school for computer science. Most of what I ship now is the same instinct from that job (measure before trusting a default, verify before calling something done) applied to LLM-based systems instead of classification models.

## Projects

- [ALIGN — AI Fitness Coaching Platform](#align--ai-fitness-coaching-platform)
- [RxGene: Pre-Prescription Pharmacogenomics Check (Hackachusetts 2026)](#rxgene-pre-prescription-pharmacogenomics-check-hackachusetts-2026)
- [Site Safety Watch (Dell x NVIDIA GB10 Hackathon)](#site-safety-watch-dell-x-nvidia-gb10-hackathon)
- [Canary Pact: AI Decision Simulator (Hackathon)](#canary-pact-ai-decision-simulator-hackathon)
- [AI Study Tutor (in progress)](#ai-study-tutor-in-progress)
- [Boston Housing Regression](#boston-housing-regression)

### ALIGN — AI Fitness Coaching Platform

> A coach that watches, listens, and adapts.

Full-stack AI fitness coaching app pairing a Claude-powered agent with real computer vision, a from-scratch RAG pipeline, and a deterministic fitness-fatigue-injury-risk model. Deployed live on Render and Vercel, not a local demo.

**The part I'd talk about in an interview:** ChromaDB's default embedding model truncates at 128 tokens. I found that out by measuring it against real coaching-note lengths, not by reading a warning in the docs, and switched to BAAI/bge-small-en-v1.5 only after confirming it fit the longest real document with margin. The retrieval relevance threshold (0.4 cosine distance) came from measuring where correct, wrong-topic, and unrelated matches actually land, not a tutorial default. Separately, I found and closed a passwordless-auth vulnerability in the Google OAuth flow before public launch, and fixed a CUDA/port-binding cold-start failure on Render by pinning a CPU-only build.

`FastAPI` `React` `PostgreSQL` `Claude API` `MediaPipe` `ChromaDB` `Google OAuth`

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_API-D97757?style=flat&logo=anthropic&logoColor=white)

### RxGene: Pre-Prescription Pharmacogenomics Check (Hackachusetts 2026)

> Your genes don't change. Your prescriptions do.

When a clinician adds a medication, RxGene re-checks the patient's existing genetic test results against CPIC guidelines and their current medications. That catches phenoconversion: a patient who is genetically a normal metabolizer but behaves like a poor one because another drug blocks the enzyme. Built by a three-person team in the Biotech & Healthcare track. I owned the engine, APIs, consult agent, tests and UI integration, built with Kiro CLI one scoped brief at a time, and nothing was committed until all 26 hand-reviewed test patients passed.

[Repo](https://github.com/hemnaath04/rxgene) · [Live demo](https://rxgene.vercel.app)

`TypeScript` `React` `CDS Hooks` `openFDA` `Kiro CLI`

### Site Safety Watch (Dell x NVIDIA GB10 Hackathon)

> An always-on safety agent that watches site cameras, spots a blocked exit, and posts it to Slack with the evidence frame, the OSHA rule and a fix to approve.

All inference runs locally on one Dell Pro Max with GB10, so raw video never leaves the box. I owned the Watcher, the component that turns a camera stream into clean, de-duplicated hazard events: 18 Python modules covering frame sampling, a motion gate, the local vision client, validation, de-duplication, the SQLite store and the CLI the agent calls.

[Repo](https://github.com/hemnaath04/site-safety-watch)

`Python` `OpenCV` `vLLM (Qwen3 35B NVFP4)` `SQLite`

### Canary Pact: AI Decision Simulator (Hackathon)

> Shows what a proposed cost cut would break before anyone approves it.

Department AI agents investigate a modeled company and surface the dependencies a spreadsheet misses. I owned the company model the simulation runs on: 156 typed entities and 121 edges across 9 departments, generated deterministically so every run reproduces byte for byte, with a load-bearing dependency planted outside the edge list so the agents are scored on what they discover.

`Python` `Pydantic` `JSON Schema` `multi-agent LLM simulation`

### AI Study Tutor (in progress)

> Still in early scoping, not shipped yet.

A LangGraph-based tutor combining Bayesian Knowledge Tracing (BKT) for skill modeling, FSRS for spaced-repetition scheduling, and pgvector for retrieval.

`LangGraph` `BKT` `FSRS` `pgvector`

### Boston Housing Regression

> A reference piece, not a headline project.

Classical ML artifact: regression modeling and feature engineering on the Boston housing dataset. Kept around as a foundational-methods reference, not something I lead with.

`Python` `Regression` `Feature Engineering`

## What I actually use

**Every day:** Python, FastAPI, React, PostgreSQL, Claude API / LLM tool-use

**AI/ML:** RAG pipelines, embeddings, agent orchestration, pose estimation (MediaPipe), vector DBs (ChromaDB), LangGraph

**Comfortable with:** Java, JavaScript, Node.js, SQL, MySQL, MongoDB

## Before this

Mad Street Den (View.AI), Chennai — AI Product Operations & Quality Analyst, ~2.5 years, owning classification-model quality and delivery for nine enterprise retail clients across seven countries at a 95%+ accuracy bar.

Now: MS in Computer Science, Northeastern University (Khoury College), Jan 2026 – May 2028, and teaching assistant for Human-Centered AI (ARTG 6460).

## Talk to me

📧 murugeshmithuna@gmail.com
💼 [linkedin.com/in/mithunamurugesh98](https://linkedin.com/in/mithunamurugesh98)
🐙 [github.com/murugeshmithuna](https://github.com/murugeshmithuna)
