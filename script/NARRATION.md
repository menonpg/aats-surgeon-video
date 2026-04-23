# Full Narration Script
# AI for Surgeons: A Practical Toolkit
# AATS Annual Meeting 2026 | 15 Minutes | Prahlad Menon
# ~2,250 words @ 150 wpm

---

## [SECTION 1 — HOOK] ~1 min / ~150 words

Something fundamental shifted in AI over the last 18 months.

Not incrementally. Fundamentally.

The models that were impressive novelties in 2023 are now capable of writing your grant applications, interpreting CT scans, simplifying radiology reports, generating a full research presentation from a single abstract, and having a fluent clinical conversation with a patient about goals of care — without a human in the loop.

And the pace isn't slowing down.

In cardiothoracic surgery specifically, the tools available to you right now can eliminate 20 to 40 percent of documentation time, accelerate literature review by an order of magnitude, and augment imaging interpretation in ways that were science fiction three years ago.

This session is not about what AI might do someday. It's about what you can use on Monday morning.

Let's go.

---

## [SECTION 2 — AI LANDSCAPE & LLMs] ~2 min / ~300 words

There are four frontier AI models you need to know right now.

**Claude Opus 4.6** from Anthropic leads on complex reasoning and has a one-million token context window — meaning you can feed it an entire textbook, or a year of operative reports, in a single prompt.

**ChatGPT 5.2** from OpenAI remains the best for structured writing — manuscripts, grant narratives, letters of recommendation.

**Gemini 3.1 Pro** from Google is multimodal, connected to live search, and can interpret images alongside text. You can show it a CT scan and ask clinical questions.

**Grok 4.20** from xAI is fast, direct, and particularly useful for technical tasks and uncensored reasoning.

Here's the critical insight: all four are now excellent. The difference between a mediocre AI result and a genuinely useful one comes almost entirely from *how you prompt it*.

A vague prompt gets a vague answer. A structured prompt — with role, context, specific task, format, and constraints — gets something dramatically better.

Instead of: *"write a patient letter about my findings"* —

Try: *"You are a thoracic surgeon. Write a one-page letter to a 67-year-old patient explaining that their CT scan shows a 1.2cm right lower lobe nodule requiring 3-month follow-up. Use plain language, 7th grade reading level. Include: what was found, why follow-up is needed, what to expect next."*

That's the difference between generic text and something you'd actually send.

We'll demonstrate this live during the session — the same surgical prompt, four models, side by side, so you can see the differences directly.

---

## [SECTION 3 — LITERATURE SEARCH] ~1.5 min / ~225 words

If you're still doing literature searches the traditional way — PubMed keyword queries, manual abstract screening — you're leaving a significant productivity advantage on the table.

**Open Evidence** answers clinical questions grounded in peer-reviewed literature with clickable citations. Ask it: *"What is the current evidence on ECMO as a bridge to transplant in adults?"* — you get a synthesized answer with sources, not a list of 200 papers to skim.

**Consensus** and **Elicit** do similar things for systematic review acceleration — surfacing the most relevant evidence automatically, clustering themes, and flagging contradictions.

The clinical impact is now quantified. A Lancet meta-analysis published this year — 38 studies, 13,000 reports, 508 evaluators — showed LLMs improve patient-perceived understanding of radiology reports by 87 percent. Reading level drops from university-grade to 7th grade. Clinician accuracy ratings: 4.45 out of 5.

The caveat is real: approximately 1 percent of AI-simplified reports contain clinically significant errors. At volume — thousands of reports per month per department — that's dozens of potentially harmful miscommunications. Human review isn't optional. But the productivity gain is undeniable, and the trajectory is clear.

---

## [SECTION 4 — SURGEON WORKFLOWS] ~2 min / ~300 words

Dr. Ghanta will walk through his personal workflow in detail. Let me give you the technical layer underneath it.

**AI scribes** — tools like Ambient Clinical Intelligence from Nuance or Nabla — listen to your patient encounter and produce a structured clinical note. The published evidence shows 20 to 40 percent reduction in documentation time. Some surgeons report leaving clinic on time for the first time in years.

Beyond notes: paste an operative report into Claude, ask for the correct procedure codes. Give it five bullet points about a resident, ask for a letter of recommendation. Upload your specific aims, ask for a grant narrative outline.

A paper published this year in Nature npj Digital Medicine showed vision-enabled AI scribes — Gemini combined with Ray-Ban Meta glasses — can document medication histories during patient encounters by reading labels in real time. That's where documentation is heading: ambient, continuous, invisible.

For research: upload a CSV of patient outcomes to ChatGPT Data Analyst and ask for survival curves, multivariate regression, subgroup analysis, and publication-ready figures. No R. No Python. No biostatistician required for early-stage analysis.

For presentations: **Kimi** generates a full conference deck from an abstract in roughly 60 seconds — charts, citations, speaker notes. Upload your abstract and figures, describe your audience, receive a complete deck.

And just to put a number on the personalized medicine frontier: a 17-year machine learning engineer named Paul Conyngham sequenced his rescue dog's tumor DNA, used AlphaFold and a custom ML pipeline, and produced a personalized mRNA cancer vaccine for $3,000. The tumor shrank 75 percent in a month. The same pipeline — AlphaFold, OpenAI, open-source bioinformatics — is available to anyone with a university computing account and a credit card.

---

## [SECTION 5 — RAG AND YOUR OWN KNOWLEDGE BASE] ~2 min / ~300 words

This is the capability that most clinicians haven't encountered yet, and it may be the most powerful one on this list.

**RAG — Retrieval-Augmented Generation** — lets you build a searchable knowledge base from *your own* documents: operative reports, research papers, institutional protocols, clinical guidelines. And then ask natural-language questions that are answered from *your* data — not from the open internet, not from hallucinated training memory.

The architecture: your documents are converted into mathematical representations called embeddings, stored in a vector database, retrieved at query time, and injected as context into the AI's response. The answer is grounded in what you actually gave it.

In 2026, RAG has evolved considerably. **GraphRAG** builds knowledge graphs for complex relational data — useful when connections between findings, medications, and outcomes matter. **Agentic RAG** uses autonomous agents to search and reason across sources. **Multimodal RAG** handles images alongside text.

And a newer approach called **Recursive Language Models — RLMs** — solves a persistent problem called context rot: as you load more documents into a prompt, AI performance degrades. RLMs process large document sets recursively, enabling reasoning over datasets too large for any single context window. For a surgical team with years of operative records and a large research corpus, this is significant.

In the session, we'll demonstrate a live RAG system built on a real cardiothoracic surgery paper corpus. You'll be able to ask it clinical questions and see exactly how retrieval and generation work together.

---

## [SECTION 6 — MEDICAL IMAGING AI] ~1.5 min / ~225 words

**Medical SAM 2** — based on Meta's Segment Anything Model — treats a 3D CT or MRI scan as a video sequence. Segment one slice, and the model propagates that segmentation automatically through the entire volume. Consistent 3D annotation without slice-by-slice manual work. Directly applicable to surgical planning, teaching cases, and rapid second opinions.

**BrainIAC**, published in Nature Neuroscience this February, pushed further. A foundation model trained on 49,000 brain MRIs — with no labels at all. Self-supervised learning. It outperforms supervised models on tumor segmentation, stroke prediction, and brain age estimation, particularly in low-data settings. The annotation bottleneck that has constrained medical AI is breakable.

And published this week: **APOLLO** — a multimodal temporal foundation model trained on 25 billion clinical events from 7.2 million patients, across 33 years of longitudinal hospital records and 28 data modalities. Labs, clinical notes, pathology images, medications, diagnoses — all unified into a single representation. What APOLLO produces is what the authors call a virtual patient: a computable embedding that captures not just the current clinical state, but the full trajectory of how that patient got there.

The implications for risk prediction, treatment response modeling, and clinical trial matching are substantial. This is the foundation model moment that medicine has been waiting for.

---

## [SECTION 7 — DATA ANALYSIS] ~1 min / ~150 words

Two specific capabilities that remove the traditional barriers to quantitative research.

For data analysis: paste a CSV of patient outcomes into ChatGPT Data Analyst or Claude. Ask for Kaplan-Meier survival curves, multivariate logistic regression, subgroup comparisons, and publication-ready figures. You get working statistical analysis — no statistical software license, no programming background required. For hypothesis generation and early-stage analysis, this is genuinely transformative.

For presentations: **Gamma** and **Beautiful.ai** generate structured visual decks from your content in minutes. And **Kimi** — the current best-in-class tool for slide generation — creates complete conference presentations from a single abstract. Upload your key figures, describe your audience, receive a full deck with surgical diagrams and speaker notes in roughly 60 seconds.

These are not future capabilities. They work today with a free or low-cost subscription.

---

## [SECTION 8 — IMAGE AND VIDEO GENERATION] ~1 min / ~150 words

For surgical education materials, conference posters, and teaching illustrations — **Gemini 3.1 Flash Image**, which went viral under the name Nano Banana 2, generates high-quality anatomical diagrams, surgical illustrations, and infographics from text descriptions. It supports subject consistency across multiple frames and produces 4K resolution outputs.

Describe the anatomy you need illustrated. Describe the procedure schematic. Get a professional-quality image in seconds, without a medical illustrator.

On the video side: tools like **HyperFrames** let an AI coding agent write and render HTML-based video compositions directly to MP4. **ArcReel** takes a story or script and produces a complete short video with consistent characters and scene assembly. **NotebookLM's Cinematic Video Overviews** — now in Google AI Ultra — can take any document and produce a narrated video with fluid animations in under an hour.

The barriers between "I have an idea" and "I have a video" are collapsing.

---

## [SECTION 9 — VOICE AGENTS, soul.py, GRACE, AND AATS AQG] ~2 min / ~300 words

I want to close with something I've been building directly — because it connects everything we've discussed, and it represents where clinical AI is actually going.

The foundation is a real-time voice communication framework called **LiveKit** — open-source, production-grade, used in clinical applications. On top of it, you layer speech recognition, a large language model, and the RAG and RLM retrieval architectures we discussed earlier.

The memory problem in clinical AI — how does an AI agent remember what a patient said in the last session, across sessions, over months — is solved by a memory architecture we published on PyPI as **soul.py**. The system uses two layers: a structured identity file containing persistent clinical facts, and a semantic retrieval layer that searches across the full conversation history. The AI doesn't forget between sessions. It knows what was said last time, and it adapts.

What this looks like in practice: an AI agent conducting goals-of-care conversations with patients with serious illness. The agent can explain what a DNR means, what POLST forms are, what palliative care involves — in plain language, adapted to the specific patient's concerns, with memory of everything discussed in prior sessions. A pilot who asks about what happens if he can't fly again gets a different conversation than a 78-year-old asking about nursing home care.

And for this audience specifically: we rebuilt the AATS Quality Gateway risk calculator as a conversational AI system called **AskAQG**. A clinician describes a patient in natural language — "65-year-old male, CABG, history of diabetes, transfer with prolonged pre-operative stay" — and the system extracts variables, makes reasonable assumptions for missing data, and returns risk predictions for operative mortality, stroke, renal failure, prolonged length of stay, and four other endpoints. Instantly. Conversationally. With what-if scenario comparison.

The combination of voice, persistent memory, and clinical knowledge bases is producing tools that feel qualitatively different from anything that existed three years ago.

---

## [SECTION 10 — WHAT TO DO MONDAY] ~1 min / ~150 words

Here's the practical takeaway.

You don't need to become an AI engineer. You need five things:

**One**: A Claude or ChatGPT Pro subscription. Fifteen to twenty dollars a month. Start there.

**Two**: A structured prompting template for your most common tasks — patient letters, operative notes, literature questions. Spend 30 minutes this weekend writing them. You'll use them for years.

**Three**: Open Evidence bookmarked. Use it for your next clinical question instead of PubMed. See the difference.

**Four**: One dataset — anything you've been meaning to analyze. Upload it to ChatGPT Data Analyst this week.

**Five**: Come back to the resources at learn.aatsqualitygateway.org. The RAG demo, the playgrounds, the deep-dives are all there and accessible with the pre-configured API keys we've set up for this session.

The tools are ready. The question is whether you are.

---

*Total: ~2,250 words | ~15 minutes @ 150 wpm*
*Speaker: Prahlad Menon*
*AATS Annual Meeting 2026 | Chicago | May 2, 7:30–9:00 AM*
