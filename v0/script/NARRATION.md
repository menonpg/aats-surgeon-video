# Full Narration Script — UPDATED WITH RESEARCH
# AI for Surgeons: A Practical Toolkit
# AATS Annual Meeting 2026 | 15 Minutes | Prahlad Menon
# ~2,250 words @ 150 wpm

---

## [SECTION 1 — HOOK] ~1 min

Something fundamental shifted in AI over the last 18 months.

Not incrementally. Fundamentally.

A systematic review published in Medical Sciences this March — 67 studies across two decades of cardiothoracic surgical AI — concluded that we have crossed a threshold: AI now enhances risk prediction, imaging interpretation, and early complication detection at a level that is changing clinical practice. Not might change. Is changing.

The FDA has issued over 1,200 breakthrough device designations to AI tools since 2016 — and the bar has moved. Algorithms that simply improve a doctor's capabilities are no longer enough. The FDA is now prioritizing AI that solves problems physicians simply *can't* — detecting multiple cancers from a single image, predicting death risk from heart failure years in advance.

This session is not about what AI might do someday. It's about what you can use on Monday morning.

Let's go.

---

## [SECTION 2 — AI LANDSCAPE & LLMs] ~2 min

There are four frontier AI models you need to know right now.

**Claude Opus 4.6** from Anthropic leads on complex reasoning and has a one-million token context window — meaning you can feed it an entire textbook, or a full year of operative reports, in a single prompt.

**ChatGPT 5.2** from OpenAI remains the best for structured writing — manuscripts, grant narratives, letters of recommendation.

**Gemini 3.1 Pro** from Google is multimodal, connected to live search, and can interpret images alongside text. You can show it a CT scan and ask clinical questions in natural language.

**Grok 4.20** from xAI is fast, direct, and particularly useful for technical and analytical tasks.

Here's the critical insight: all four are now excellent. The difference between a mediocre AI result and a genuinely useful one comes almost entirely from *how you prompt it*.

A vague prompt gets a vague answer. A structured prompt — with role, context, specific task, format, and constraints — gets something dramatically better.

Instead of: *"write a patient letter about my findings"* —

Try: *"You are a thoracic surgeon. Write a one-page letter to a 67-year-old patient explaining that their CT scan shows a 1.2cm right lower lobe nodule requiring 3-month follow-up. Use plain language, 7th grade reading level. Include what was found, why follow-up is needed, and what to expect next."*

That's the difference between generic text and something you'd actually send.

We'll demonstrate this live — same surgical prompt, four models, side by side.

---

## [SECTION 3 — LITERATURE SEARCH] ~1.5 min

If you're still doing literature searches the traditional way — PubMed keyword queries, manual abstract screening — you're leaving significant time on the table.

**Open Evidence** answers clinical questions grounded in peer-reviewed literature with clickable citations. Ask it: *"What is the current evidence on ECMO as a bridge to transplant in adults?"* — you get a synthesized answer with sources, not 200 papers to skim.

**Consensus** and **Elicit** do similar things for systematic review acceleration — surfacing the most relevant evidence automatically, clustering themes, flagging contradictions across studies.

A new AI framework published this month can now automatically label radiology images at scale — addressing what has been the single biggest bottleneck in medical AI development: the need for expert annotation. This changes the economics of building clinical AI tools fundamentally.

The clinical impact of AI-assisted communication is now quantified. A Lancet meta-analysis — 38 studies, 13,000 reports, 508 evaluators — showed LLMs improve patient-perceived understanding of radiology reports by 87 percent. Reading level drops from university-grade to 7th grade. Clinician accuracy ratings: 4.45 out of 5. With a caveat: about 1 percent contain clinically significant errors. Human review isn't optional. But the productivity gain is real and documented.

---

## [SECTION 4 — SURGEON WORKFLOWS] ~2 min

Dr. Ghanta will walk through his personal workflow. Let me give you the technical layer underneath it.

**AI scribes** — tools like Ambient Clinical Intelligence or Nabla — listen to your patient encounter and produce a structured clinical note. Published evidence: 20 to 40 percent reduction in documentation time. Some surgeons report leaving clinic on time for the first time in years.

Beyond notes: paste an operative report into Claude, ask for procedure codes. Give it five bullet points about a resident, ask for a letter of recommendation. Upload your specific aims, ask for a grant narrative outline.

Vision-enabled AI scribes published this year in Nature npj Digital Medicine — Gemini combined with wearable cameras — can document medication histories *during* encounters by reading labels in real time. The March 2026 systematic review on cardiothoracic surgery AI specifically highlights AI-assisted intraoperative guidance and early complication detection as areas where augmented reality combined with AI is now changing surgical execution.

For research: upload a CSV of patient outcomes to ChatGPT Data Analyst. Ask for Kaplan-Meier curves, multivariate regression, subgroup analysis, publication-ready figures. No R. No Python. No biostatistician required for early-stage analysis.

For presentations: **Kimi** generates a full conference deck from an abstract in roughly 60 seconds — charts, citations, speaker notes included.

And on the frontier of personalized medicine: a machine learning engineer named Paul Conyngham used AlphaFold and a custom pipeline to design a personalized mRNA cancer vaccine for his dog for $3,000. The tumor shrank 75 percent in a month. The same tools — AlphaFold, open-source bioinformatics, publicly available compute — are accessible to any surgeon with a research question and a university account.

---

## [SECTION 5 — RAG AND YOUR OWN KNOWLEDGE BASE] ~2 min

This is the capability that most clinicians haven't encountered yet, and it may be the most powerful one on this list.

**RAG — Retrieval-Augmented Generation** — lets you build a searchable knowledge base from *your own* documents: operative reports, research papers, institutional protocols, clinical guidelines. Ask natural-language questions answered from *your* data — not the open internet, not hallucinated memory.

The architecture: your documents are converted into mathematical representations called embeddings, stored in a vector database, retrieved at query time, and injected as context into the AI's response. Grounded answers, verifiable sources.

In 2026, RAG has matured significantly. **GraphRAG** builds knowledge graphs for complex relational data — critical when connections between diagnoses, medications, and outcomes matter more than individual facts. **Agentic RAG** uses autonomous agents to search and reason across multiple sources. **Multimodal RAG** handles images alongside text — relevant for operative reports that reference imaging.

And a newer approach called **Recursive Language Models — RLMs** — solves a persistent problem called context rot: as you load more documents into a prompt, AI performance degrades. RLMs process large document sets recursively, enabling coherent reasoning over datasets too large for any context window. For a surgical research group with years of operative records and a substantial paper corpus, this is significant.

We'll demonstrate a live RAG system during the session — a real cardiothoracic surgery paper corpus, searchable by natural language, with verifiable citations.

---

## [SECTION 6 — MEDICAL IMAGING AI] ~1.5 min

The systematic review published last month in Medical Sciences documented AI's role across the full imaging pipeline in cardiothoracic surgery: preoperative planning, intraoperative guidance, postoperative monitoring. This is not experimental — it is current practice at leading centers.

**Medical SAM 2** — based on Meta's Segment Anything Model — treats a 3D CT or MRI scan as a video. Segment one slice, and the model propagates that segmentation automatically through the entire volume. Consistent 3D annotation without slice-by-slice manual work. Directly applicable to surgical planning, teaching, and rapid second opinions.

**BrainIAC**, published in Nature Neuroscience this February, took a different approach: a foundation model trained on 49,000 brain MRIs with *no labels at all*. Self-supervised learning. It outperforms supervised models on tumor segmentation, stroke prediction, and brain age estimation, particularly in low-data settings. The annotation bottleneck has been broken.

And published this week: **APOLLO** — trained on 25 billion clinical events from 7.2 million patients across 33 years of longitudinal hospital records and 28 data modalities. What APOLLO produces is a virtual patient: a computable embedding that captures not just the current clinical state, but the full trajectory of how that patient got there — labs, notes, pathology images, medications, diagnoses, all unified. The implications for risk prediction, treatment response modeling, and trial matching are substantial.

The FDA now recognizes this category: AI that solves problems physicians simply *can't*, at scale, in real time. That is no longer a future state.

---

## [SECTION 7 — DATA ANALYSIS] ~1 min

Two capabilities that remove traditional barriers.

For analysis: paste a CSV of patient outcomes into ChatGPT Data Analyst or Claude. Ask for Kaplan-Meier survival curves, multivariate logistic regression, subgroup comparisons, publication-ready figures. Working statistical analysis — no statistical software license, no programming background required. For hypothesis generation, this is transformative.

For presentations: **Gamma** and **Beautiful.ai** generate structured visual decks from your content in minutes. And **Kimi** creates complete conference presentations from a single abstract — surgical diagrams, structured slides, speaker notes — in roughly 60 seconds.

These work today with a $20/month subscription.

---

## [SECTION 8 — IMAGE AND VIDEO GENERATION] ~1 min

For surgical education materials, conference posters, teaching illustrations — **Gemini 3.1 Flash Image** (which went viral as Nano Banana 2) generates high-quality anatomical diagrams and infographics from text descriptions, at up to 4K resolution with subject consistency.

Describe the anatomy. Describe the procedure schematic. Get a professional-quality illustration in seconds.

On the video side: tools like **HyperFrames** let an AI coding agent write and render HTML-based video compositions to MP4. **NotebookLM's Cinematic Video Overviews** take any document — a research paper, a clinical guideline — and produce a narrated video with fluid animations in under an hour. The barriers between "I have content" and "I have a video" are collapsing.

---

## [SECTION 9 — VOICE AGENTS, soul.py, GRACE, AND AATS AQG] ~2 min

I want to close with systems I've been building directly — because they connect everything we've discussed, and represent where clinical AI is actually going.

The foundation is a real-time voice communication framework called **LiveKit** — open-source, production-grade, used in clinical applications. On top of it: speech recognition, a large language model, and the RAG and RLM retrieval architectures we just discussed.

The memory problem in clinical AI — how does an agent remember what a patient said last session, across months — is solved by a memory architecture we published as **soul.py** on PyPI. Two layers: a structured identity file with persistent clinical facts, and semantic retrieval across the full conversation history. The AI doesn't forget. It knows what was discussed in the last session, and it adapts accordingly.

In practice: an AI agent conducting goals-of-care conversations with patients with serious illness. The agent explains what a DNR means, what POLST forms are, what palliative care involves — in plain language, adapted to the specific patient's life context, with full memory across sessions. The routing is entirely LLM-driven: the agent classifies whether a question requires clinical guidelines, session history, or both — before it retrieves anything.

For cardiothoracic surgery specifically: we rebuilt the AATS Quality Gateway risk calculator as a conversational AI system — **AskAQG**. A clinician describes a patient in natural language: *"65-year-old male, CABG, history of diabetes, transfer with prolonged pre-op stay."* The system extracts variables, makes reasonable assumptions for missing data, and returns risk predictions for operative mortality, stroke, renal failure, prolonged length of stay, and four other endpoints. Instantly. Conversationally. What-if scenarios included.

The LITE Calculator takes this further for thoracic surgery: voice input, 37 fields auto-populated from clinical notes, with full PDF and CSV export of the risk summary.

The combination of voice, persistent memory, LLM-based routing, and clinical knowledge bases is producing tools that feel qualitatively different from anything that existed three years ago — and the architecture is reproducible.

---

## [SECTION 10 — WHAT TO DO MONDAY] ~1 min

Here's the practical takeaway. Five things:

**One**: A Claude or ChatGPT Pro subscription. Fifteen to twenty dollars a month. Start today.

**Two**: Write three prompt templates for your most common tasks this weekend — patient letters, literature questions, operative summaries. You'll use them for years.

**Three**: Bookmark Open Evidence. Use it for your next clinical question instead of PubMed. See the difference.

**Four**: One dataset. Upload it to ChatGPT Data Analyst this week. Ask it for something you've been meaning to analyze.

**Five**: learn.aatsqualitygateway.org — the playgrounds, RAG demo, and deep-dives are all there, with pre-configured API keys set up for this session.

The tools are ready. They're documented, they're accessible, and the evidence base is growing.

The question is whether you'll be the surgeon who uses them.

---

*~2,300 words | ~15 minutes @ 150 wpm*
*Speaker: Prahlad Menon | AATS Annual Meeting 2026 | Chicago | May 2, 7:30–9:00 AM*

## RESEARCH CITATIONS USED
- Streian et al., Medical Sciences 14(2):164 (2026) — systematic review, 67 studies, AI in CT surgery
- STAT News / FDA Breakthrough Device Tracker (Apr 2026) — 1,200+ AI breakthrough designations
- Lancet meta-analysis — LLMs + radiology reports, 87% comprehension improvement
- Nature npj Digital Medicine (2026) — vision-enabled AI scribes, Gemini + Ray-Ban
- Nature Neuroscience (Feb 2026) — BrainIAC, 49K unlabeled MRIs
- arXiv 2604.18570 (Apr 2026) — APOLLO, 25B events, 7.2M patients
- Crescendo AI / radiology auto-labeling framework (Apr 2026)
- Paul Conyngham / Rosie cancer vaccine (Mar 2026)
