# Hi, I'm Subamithuna Murugesh

> Looking for AI engineering internships/co-ops starting **January 2027**
> 📍 Boston, MA · 🎓 MS CS @ Northeastern Khoury (started Spring 2026, graduating May 2028)
> 🛂 F-1 visa, authorized to work in the US via CPT/OPT for internships and co-ops

I spent two and a half years running applied ML pipelines for nine enterprise retail clients before deciding I wanted to build the systems instead of operating them, so I went back to school for computer science. Most of what I ship now is the same instinct from that job (measure before trusting a default, verify before calling something done) applied to LLM-based systems instead of classification models.

## Projects

- [ALIGN — AI Fitness Coaching Platform](#align--ai-fitness-coaching-platform)
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

Mad Street Den (View.AI), Chennai — AI Product Operations & Quality Analyst, ~2.5 years, owning classification-model quality and delivery across nine enterprise clients (Saks Fifth Avenue, Inditex/Zara, PVH, Fairprice, Landmark, Azadea) at a 95%+ accuracy bar.

Now: MS in Computer Science, Northeastern University (Khoury College), Jan 2026 – May 2028.

## Talk to me

📧 murugeshmithuna@gmail.com
💼 [linkedin.com/in/mithunamurugesh98](https://linkedin.com/in/mithunamurugesh98)
🐙 [github.com/murugeshmithuna](https://github.com/murugeshmithuna)
