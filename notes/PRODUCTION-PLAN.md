# Slide-by-Slide Production Plan
# Visual + Narration mapping for HyperFrames / HTML→MP4 pipeline
# AATS Branding: Black bg / AATS Red #CC0000 / White text

---

## BRANDING TOKENS
```
bg:        #0A0A0A (near-black)
accent:    #CC0000 (AATS red)
text:      #FFFFFF
subtext:   #AAAAAA
font:      Inter, system-ui
logo:      AATS Quality Gateway wordmark + icon
```

---

## SLIDE 1 — Title Card [6s]
- AATS logo top-left
- Center: "AI for Surgeons: A Practical Toolkit"
- Sub: "AATS Annual Meeting 2026 | May 2, Chicago"
- Animated red underline reveal

## SLIDE 2 — The Shift [20s]
- Timeline 2023 → 2024 → 2025 → 2026
- Each year: key AI milestone pops in
- End frame: "Not incremental. Fundamental."
- Red accent border left

## SLIDE 3 — The Four Frontier Models [30s]
- 4-quadrant dark grid
- Claude / ChatGPT / Gemini / Grok — logo + 1-liner each
- Red highlight: "All now excellent. The difference is how you use them."
- Source: learn.aatsqualitygateway.org/ai-playground/lesson5

## SLIDE 4 — Prompting: Before / After [25s]
- Split screen
- Left (grey, dim): vague prompt → mediocre output
- Right (white, bright): structured prompt → surgical letter
- AATS red arrow separating them

## SLIDE 5 — Literature Search [20s]
- Screenshot: Open Evidence answering "ECMO bridge to transplant"
- Stat overlay (red badge): "87% improvement in patient understanding"
- Sub: "Lancet meta-analysis 2026 | 38 studies | 13,000 reports"

## SLIDE 6 — AI Scribes & Documentation [25s]
- Split: surgeon in clinic (left) → structured note (right)
- Stat: "20–40% reduction in documentation time"
- Bottom ticker: "Nature npj Digital Medicine 2026 — vision-enabled scribes"

## SLIDE 7 — Surgeon Research Workflows [20s]
- 4 icons in row: CSV → Chart | Abstract → Slides | Bullets → Grant | Notes → Codes
- Tool names: ChatGPT Data Analyst | Kimi | Claude Opus 4.6
- AATS red section header: "Research & Documentation"

## SLIDE 8 — Rosie: Personalized Medicine [18s]
- Stat card: "$3,000. AlphaFold. mRNA vaccine. Tumor ↓75%."
- Caption: "The same pipeline is available to anyone with a university computing account."

## SLIDE 9 — RAG Architecture [30s]
- Animated flow (left to right):
  Documents → [Embeddings] → Vector DB → Query → [LLM] → Answer
- Labels: RAG | GraphRAG | Agentic RAG | RLM
- Red highlight: "Your data. Not the internet."
- Source: blog.themenonlab.com/blog/rag-plus-rlm-complete-knowledge-base-architecture

## SLIDE 10 — Medical SAM 2 [20s]
- CT scan slice → segmentation propagation animation (3D volume)
- Caption: "Segment one slice. Model propagates through the entire volume."
- Red badge: "Meta SAM 2 adapted for medical imaging"

## SLIDE 11 — BrainIAC [18s]
- Brain MRI → model outputs (tumor, stroke, age)
- Stat: "49K unlabeled MRIs. Zero annotations."
- Red badge: "Nature Neuroscience | Feb 2026"

## SLIDE 12 — APOLLO [25s]
- Infographic: 4 large numbers
  25B events | 7.2M patients | 28 modalities | 33 years
- Quote: "A virtual patient — not just what is happening, but how they got there."
- Red badge: "arXiv 2026 | Faisal Mahmood Lab"
- Source: blog.themenonlab.com/blog/apollo-multimodal-temporal-foundation-model-healthcare

## SLIDE 13 — Image & Video Generation [20s]
- Left: text prompt → surgical diagram (Nano Banana 2)
- Right: abstract → slide deck (Kimi, 60 seconds)
- Caption: "From idea to visual in seconds."

## SLIDE 14 — Voice Agent Architecture [25s]
- Animated diagram:
  🎤 Mic → STT → [LLM + RAG/RLM] → TTS → 🔊 Patient
- Labels: LiveKit | Deepgram | Azure OpenAI | Qdrant | Azure TTS
- Caption: "Real-time voice. Persistent memory. Clinical knowledge base."

## SLIDE 15 — Grace: Goals of Care Voice Agent [25s]
- Audio waveform animation
- Transcript excerpt (generic, no institution):
  Patient: "What happens if I can't breathe on my own?"
  Grace: "That's an important question. Let me explain what a ventilator is..."
- Caption: "Adapts to each patient. Remembers every session."
- Red badge: "soul.py — persistent AI memory | pip install soul-agent"

## SLIDE 16 — AATS AQG: Conversational Risk Assessment [25s]
- Screenshot: AskAQG conversation + risk prediction table
- Highlight row: "Operative Mortality: 0.16%"
- Caption: "From natural language to 8 surgical risk predictions — no form filling."
- Source: themenonlab.com/quantmd/aats
- Button: riskcalculator.aatsqualitygateway.org

## SLIDE 17 — LITE Calculator [20s]
- Screenshot: LITE interface (37 fields auto-populated, AI chat panel)
- Caption: "Paste clinical notes. Voice input. AI extracts all 37 variables."
- Red badge: "Thoracic Surgery | Lung + Esophageal"

## SLIDE 18 — What To Do Monday [20s]
- 5-point checklist (checkboxes animate in, AATS red)
  ✓ Claude / ChatGPT Pro ($20/mo)
  ✓ Write 3 prompt templates this weekend
  ✓ Bookmark Open Evidence
  ✓ Upload one dataset to ChatGPT Data Analyst
  ✓ learn.aatsqualitygateway.org — playgrounds + demos

## SLIDE 19 — CTA / Resources [15s]
- AATS logo centered
- URL: learn.aatsqualitygateway.org
- QR code (right side)
- "Bring your laptop. Bring your hardest problem."
- Red footer: "AATS Annual Meeting 2026 | AI for Surgeons Workshop"

---

## Production Notes

### HyperFrames Setup
```bash
npx hyperframes init aats-surgeon-video
cd aats-surgeon-video
npx skills add heygen-com/hyperframes   # adds /hyperframes Claude Code skill
npx hyperframes preview                 # live preview in browser
npx hyperframes render                  # → MP4
```

### Azure TTS Voice
```python
# Voice: en-US-AndrewMultilingualNeural (professional male)
# Rate: -5% (slightly slower, clinical/authoritative)
# Script: script/NARRATION.md — split by [SECTION] markers
```

### Screenshots needed
- [ ] learn.aatsqualitygateway.org/surgeon-program — hero
- [ ] Open Evidence — cardiothoracic clinical question
- [ ] Consensus or Elicit UI
- [ ] AskAQG conversation + risk table (themenonlab.com/quantmd/aats)
- [ ] LITE Calculator interface
- [ ] Medical SAM 2 segmentation example
- [ ] learn.aatsqualitygateway.org/rag-demo
- [ ] Kimi slide generation from abstract
- [ ] ChatGPT Data Analyst with surgical CSV

### Diagrams to generate (Nano Banana 2 / Gemini Flash Image)
- [ ] RAG+RLM architecture flow
- [ ] APOLLO 4-number infographic
- [ ] Voice agent architecture
- [ ] Frontier LLM 4-quadrant grid (Claude/GPT/Gemini/Grok)
- [ ] soul.py memory architecture
