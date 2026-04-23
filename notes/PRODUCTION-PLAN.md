# Slide-by-Slide Production Plan
# Visual + Narration mapping for HyperFrames / HTML→MP4 pipeline

---

## SLIDE 1 — Title Card
**Visual:** Dark background, animated text reveal
**Text:** "AI for Surgeons: A Practical Toolkit"
**Subtext:** "AATS Annual Meeting 2026 | May 2, 2026 | Chicago"
**Duration:** 6s

## SLIDE 2 — The Shift
**Visual:** Timeline 2023→2026, key milestones appearing
**Narration:** "Something fundamental shifted..."
**Duration:** 20s

## SLIDE 3 — The Four Frontier Models
**Visual:** 4-quadrant grid: Claude / ChatGPT / Gemini / Grok with logos and 1-line description each
**Key stat:** "All frontier models are now very good — the difference is in how you use them."
**Duration:** 30s

## SLIDE 4 — Prompt Engineering (Before/After)
**Visual:** Split screen — vague prompt vs structured prompt → output quality comparison
**Source:** LLM Playground at learn.aatsqualitygateway.org/ai-playground/lesson5
**Duration:** 25s

## SLIDE 5 — AI Literature Search
**Visual:** Screenshot of Open Evidence answering a clinical question
**Stat overlay:** "87% improvement in patient understanding — Lancet meta-analysis, 38 studies"
**Duration:** 20s

## SLIDE 6 — AI Scribes & Documentation
**Visual:** Side-by-side: surgeon in clinic → structured note generated
**Stat:** "20–40% reduction in documentation time"
**Quote:** "Vision-enabled scribes (Gemini + Ray-Ban) — npj Digital Medicine 2026"
**Duration:** 25s

## SLIDE 7 — RAG Architecture
**Visual:** Animated diagram: Documents → Embeddings → Vector DB → Query → Answer
**Labels:** RAG / GraphRAG / Agentic RAG / RLM
**Source:** blog.themenonlab.com/blog/rag-plus-rlm-complete-knowledge-base-architecture
**Duration:** 30s

## SLIDE 8 — Medical SAM 2
**Visual:** CT scan slice → 3D segmentation propagation animation
**Caption:** "Segment one slice. Get consistent 3D annotation automatically."
**Source:** blog.themenonlab.com/blog/medical-sam2-3d-medical-image-segmentation
**Duration:** 20s

## SLIDE 9 — BrainIAC
**Visual:** Brain MRI → model output (tumor segmentation, age prediction)
**Stat:** "49K unlabeled MRIs. No annotations. Nature Neuroscience, Feb 2026."
**Duration:** 18s

## SLIDE 10 — APOLLO
**Visual:** Infographic: 25B events / 7.2M patients / 28 modalities / 33 years
**Quote:** "A virtual patient — not just what is happening, but how they got there."
**Source:** blog.themenonlab.com/blog/apollo-multimodal-temporal-foundation-model-healthcare
**Duration:** 25s

## SLIDE 11 — Data & Presentations
**Visual:** CSV → Kaplan-Meier curve (ChatGPT Data Analyst)
         + Abstract → Slide deck (Kimi)
**Duration:** 20s

## SLIDE 12 — Voice Agents: Architecture
**Visual:** Diagram: LiveKit → STT → LLM → RAG/RLM → TTS → Patient
**Caption:** "Real-time voice, persistent memory, clinical knowledge base"
**Duration:** 25s

## SLIDE 13 — Goals of Care Voice Agent (Generic)
**Visual:** Audio waveform + conversation transcript excerpt
**Caption:** "An AI agent that explains DNR, POLST, advance directives — and remembers."
**Note:** No institution names
**Duration:** 25s

## SLIDE 14 — AATS AQG Conversational Risk Calculator
**Visual:** Screenshot of AskAQG conversation + risk table
**Source:** themenonlab.com/quantmd/aats
**Caption:** "65yo male, CABG, diabetes → 0.16% operative mortality — from natural language"
**Duration:** 25s

## SLIDE 15 — Call to Action
**Visual:** Workshop URL + QR code
         "learn.aatsqualitygateway.org"
**Text:** "Bring your laptop. Try the tools live. Bring your hardest problem."
**Duration:** 15s

---

## Production Notes

**Tool:** HyperFrames (HeyGen) — HTML compositions → MP4
- Install: `npx hyperframes init aats-video`
- Agent: Claude Code with `/hyperframes` skill
- Render: `npx hyperframes render`

**Voice:** Azure TTS or ElevenLabs
- Voice: pre-built male (professional/warm)
- Script: script/NARRATION.md
- Generate per-section MP3s, sync with slide timing

**Screenshots needed:**
- [ ] learn.aatsqualitygateway.org/surgeon-program
- [ ] Open Evidence answering a cardiothoracic question
- [ ] AskAQG conversation (from Google Drive demo or themenonlab.com/quantmd/aats)
- [ ] LITE Calculator interface
- [ ] Medical SAM 2 segmentation example
- [ ] RAG demo from learn.aatsqualitygateway.org/rag-demo
- [ ] Kimi slide generation

**Diagrams to generate (Gemini Flash Image / Nano Banana 2):**
- [ ] RAG+RLM architecture flow
- [ ] APOLLO multimodal timeline
- [ ] Voice agent architecture
- [ ] Frontier LLM comparison grid
