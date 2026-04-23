# Video Brief — AI for Surgeons: A Practical Toolkit
# AATS Annual Meeting 2026 — Production Bible

---

## Purpose
A 15-minute narrated video overview for the AATS Annual Meeting 2026 workshop.
Aimed at cardiothoracic surgeons with little or no prior AI experience.

## Branding
- **AATS Quality Gateway** color scheme: Black background, AATS red (#CC0000), white text
- Logo: AATS AI Training Literacy & Application (from learn.aatsqualitygateway.org)
- Font style: Clean sans-serif, clinical/professional
- Lower thirds: Red accent bar, white text
- Section cards: Dark with red left border

## Audience
- Cardiothoracic surgeons
- No assumed AI background
- Interested in practical, immediately usable tools
- Chicago, May 2, 2026 — 7:30–9:00 AM

## Tone
- Authoritative but accessible
- 1 speaker: Prahlad Menon
- No jargon without explanation
- Real demos / screenshots — not fake mockups

## Production Stack
| Component | Tool |
|-----------|------|
| Video composition | HyperFrames (HTML → MP4, agent-driven) |
| Narration voice | Azure TTS (pre-built male, professional) |
| Screenshots | Live browser capture |
| Diagrams | Gemini 3.1 Flash Image (Nano Banana 2) |
| Final stitch | FFmpeg |

## Word Count Target
~2,250 words @ 150 wpm = 15 minutes

---

## Section Structure

| # | Section | Content | Duration |
|---|---------|---------|----------|
| 1 | Hook | Why AI matters for CT surgery right now | 1 min |
| 2 | AI Landscape | LLMs — what they are, frontier models, prompting | 2 min |
| 3 | Literature Search | Open Evidence, Consensus, Elicit — live screenshots | 1.5 min |
| 4 | Surgeon Workflows | Scribes, notes, letters, presentations, grants | 2 min |
| 5 | RAG + RLM | Your own knowledge base, GraphRAG, RLM breakthrough | 2 min |
| 6 | Medical Imaging AI | VLMs, SAM2, BrainIAC, APOLLO — screenshots | 1.5 min |
| 7 | Data Analysis | Spreadsheets → stats → figures, no R/Python | 1 min |
| 8 | Image & Video Gen | Nano Banana 2, surgical diagrams, Kimi slides | 1 min |
| 9 | Prahlad's Section | LiveKit voice agents, soul.py, Grace demo (generic), AATS AQG | 2 min |
| 10 | What to Do Monday | Practical takeaways + resources | 1 min |

**Total: 15 min**

---

## Section 9 — Prahlad's Section (KEY)
This is the unique differentiator — real systems we built, not demos of third-party tools.

**Topics:**
- LiveKit as the real-time voice infrastructure layer
- soul.py: persistent AI memory architecture (our PyPI package)
  - SOUL.md + MEMORY.md anchor system
  - RAG + RLM hybrid retrieval
  - Cross-session recall — the agent remembers
- Grace: a working voice AI agent for goals-of-care conversations
  - Generic / no institution name
  - Explains DNR, POLST, advance directives conversationally
  - Searches clinical KB + session history with LLM-based routing
- AATS AQG: conversational risk assessment
  - AskAQG — MCP + GPT-4o, natural language → 8 risk models
  - LITE Calculator — voice input, 37 fields auto-populated
  - Demo: "65yo male, CABG, diabetes" → operative mortality 0.16%

---

## Content Sources
- **Primary outline:** learn.aatsqualitygateway.org/surgeon-program
- **AATS AQG system:** themenonlab.com/quantmd/aats
- **Blog posts used:**
  - apollo-multimodal-temporal-foundation-model-healthcare
  - rag-plus-rlm-complete-knowledge-base-architecture
  - brainiac-self-supervised-brain-mri-foundation-model
  - medical-sam2-3d-medical-image-segmentation
  - llms-radiology-reports-lancet-meta-analysis
  - human-ai-collaboration-radiology-rethinking
  - paul-conyngham-rosie-mrna-cancer-vaccine-ai-alphafold
  - notebooklm-cinematic-video-overviews-education
  - hyperframes-claude-code-writes-renders-videos
  - arcreel-novel-to-video-multi-agent-pipeline
  - nvidia-personaplex-full-duplex-voice-ai-how-to-guide
  - local-voice-ai-complete-guide
  - fast-vad-721x-realtime-voice-activity-detection

---

## Screenshots Needed (browser capture)
- [ ] learn.aatsqualitygateway.org/surgeon-program — hero + agenda
- [ ] Open Evidence answering a cardiothoracic clinical question
- [ ] Consensus / Elicit interface
- [ ] AskAQG conversation (from themenonlab.com/quantmd/aats demo)
- [ ] LITE Calculator interface (auto-populated form)
- [ ] Medical SAM 2 segmentation (CT scan → 3D)
- [ ] learn.aatsqualitygateway.org/rag-demo
- [ ] Kimi generating slides from an abstract
- [ ] ChatGPT Data Analyst — CSV → survival curve
- [ ] Gemini Flash Image / Nano Banana 2 output

## Diagrams to Generate
- [ ] RAG+RLM architecture flow (animated)
- [ ] APOLLO: 25B events / 7.2M patients / 28 modalities infographic
- [ ] Voice agent architecture: mic → STT → LLM → RAG → TTS → speaker
- [ ] Frontier LLM comparison 4-quadrant grid
- [ ] soul.py memory architecture: SOUL.md + MEMORY.md + vector DB
