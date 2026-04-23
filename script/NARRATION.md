# Full Narration Script
# AI for Surgeons: A Practical Toolkit
# AATS Annual Meeting 2026 | 15 Minutes | 1 Speaker

---

## [SECTION 1 — INTRO & AI LANDSCAPE] ~2 min

Something fundamental shifted in AI in the last 18 months.

Not incrementally. Fundamentally.

The models that were impressive novelties in 2023 are now capable of writing grant applications, interpreting CT scans, simplifying radiology reports, generating full research presentations from an abstract, and having a fluent clinical conversation with a patient about goals of care.

And the pace isn't slowing down.

Right now, in 2026, every major frontier AI model — Claude Opus 4.6, ChatGPT 5.2, Gemini 3.1, Grok 4.20 — is genuinely good. Not good for a computer. Good. The question is no longer "can AI do this?" The question is: "are *you* using it?"

This session is about practical tools. Things you can use today, in your clinic, your OR, your research workflow — not hypothetical future systems.

We're going to cover five domains: interacting with AI models, literature search, clinical documentation and research productivity, medical imaging, and finally a category that I think will genuinely surprise you — voice AI and conversational clinical tools.

Let's go.

---

## [SECTION 2 — LLMs: COMPARING FRONTIER MODELS] ~2.5 min

The most important skill in using AI is knowing how to talk to it.

There are four frontier models you need to know right now.

**Claude Opus 4.6** from Anthropic leads on complex reasoning and has a one-million token context window — meaning you can feed it an entire book, or a year of patient records, in a single prompt.

**ChatGPT 5.2** from OpenAI is still the best for structured writing — manuscripts, grant narratives, clinical letters.

**Gemini 3.1 Pro** from Google is multimodal and connected to live search. You can show it an image and ask clinical questions.

**Grok 4.20** from xAI is fast, direct, and useful for technical tasks.

Here's the key insight: all four are now excellent. The difference in your results comes almost entirely from *how you prompt them*.

A vague prompt gets a vague answer. A structured prompt — with role, context, specific task, format, and constraints — gets a dramatically better one.

For example: instead of "write a patient letter about my findings," you say: "You are a thoracic surgeon. Write a one-page letter to a 67-year-old patient explaining that their CT scan shows a 1.2cm right lower lobe nodule requiring 3-month follow-up imaging. Use plain language at a 7th grade reading level. Include: what was found, why follow-up is needed, and what to do next."

That's the difference between generic text and something you'd actually send.

We'll demo this live in the session — same surgical prompt, four models, side by side.

---

## [SECTION 3 — AI LITERATURE SEARCH] ~1.5 min

If you're still doing literature searches the traditional way — PubMed keyword searches, manual abstract screening — you're leaving a significant productivity advantage on the table.

Three tools have changed this permanently.

**Open Evidence** answers clinical questions grounded in peer-reviewed literature with clickable citations. Ask it: "What's the current evidence on ECMO as a bridge to transplant in adults?" — and you get a synthesized answer, not a list of 200 papers to skim.

**Consensus** and **Elicit** do similar things for systematic review acceleration — taking a research question and surfacing the most relevant evidence automatically.

A Lancet meta-analysis published this year quantified something we've been seeing anecdotally: LLMs simplify radiology reports by 87% in patient-perceived understanding. Reading level drops from university-grade to 7th grade. Clinician accuracy ratings: 4.45 out of 5. That's not a pilot study — it's 38 studies, 13,000 reports, 508 evaluators.

The caveat is real: about 1% of AI-simplified reports contain clinically significant errors. At scale — thousands of reports per month per department — that's dozens of potentially harmful miscommunications. So human review isn't optional. But the productivity gain is undeniable.

---

## [SECTION 4 — AI FOR THE PRACTICING SURGEON] ~2 min

Dr. Ghanta is going to walk through his own workflow in detail. Let me give you the technical layer underneath it.

**AI scribes** — tools like Ambient Clinical Intelligence from Nuance or Nabla — listen to your patient encounter and generate a structured clinical note. Studies show 20 to 40 percent reduction in documentation time. Some surgeons report leaving clinic on time for the first time in years.

Beyond notes: you can paste an operative report into Claude and ask it to generate the correct procedure codes. You can ask it to draft a letter of recommendation given a few bullet points about the resident. You can generate a grant narrative outline from your specific aims page.

A paper published this year in Nature npj Digital Medicine showed vision-enabled AI scribes — Gemini combined with Ray-Ban Meta glasses — can document medication histories *during* patient encounters by reading labels in real time. This is where the technology is heading: ambient, invisible, continuous documentation.

On the research side: you can upload a spreadsheet of patient outcomes and ask ChatGPT Data Analyst to generate survival curves and publication-ready figures — no R, no Python, no biostatistician required.

For presentations: **Kimi** generates a full conference deck from an abstract in roughly 60 seconds. Complete with charts, citations, and speaker notes.

These aren't future capabilities. They're available today with a free or low-cost subscription.

---

## [SECTION 5 — RAG AND YOUR OWN KNOWLEDGE BASE] ~2 min

This is the one that most clinicians haven't heard about yet, and it may be the most powerful capability on this list.

**RAG — Retrieval-Augmented Generation** — lets you build a searchable knowledge base from *your own* documents. Operative reports. Research papers. Clinical guidelines. Your institution's protocols. And then ask it natural language questions that are answered from *your* data — not from the open internet.

The architecture is straightforward: your documents are converted into mathematical representations called embeddings, stored in a vector database, and retrieved at query time. The AI answers your question grounded in what you actually gave it.

In 2026, RAG has evolved significantly. **GraphRAG** builds knowledge graphs for complex relational data — useful when you need to understand connections between findings, medications, and outcomes. **Agentic RAG** uses autonomous agents to search and reason. **Multimodal RAG** handles images alongside text.

And there's a newer approach called **Recursive Language Models — or RLMs** — that solves a persistent problem in RAG called "context rot." As you load more documents into a prompt, AI performance degrades. RLMs solve this by recursively processing large document sets, effectively enabling AI reasoning over datasets too large for any single context window. For a surgical team with years of operative records and a large research corpus, this is significant.

We'll demo a live RAG system during the session — a real cardiothoracic surgery paper corpus, searchable by natural language.

---

## [SECTION 6 — MEDICAL IMAGING AI] ~2 min

This is where the biology meets the computation in the most visible way.

**Medical SAM 2** — based on Meta's Segment Anything Model — treats a 3D CT or MRI scan like a video. Segment one slice, and the model propagates that segmentation through the entire volume automatically. Consistent 3D annotation without slice-by-slice manual work. Practical for surgical planning, teaching cases, and rapid second opinions.

**BrainIAC**, published in Nature Neuroscience this February, went further. A foundation model trained on 49,000 brain MRIs — with *no labels at all*. Self-supervised learning. It outperforms supervised models on tumor segmentation, stroke prediction, and brain age estimation, especially in low-data settings. The bottleneck in medical AI has always been annotation. BrainIAC shows the bottleneck is breakable.

And just published this week — **APOLLO**: a multimodal temporal foundation model trained on 25 billion clinical events from 7.2 million patients across 33 years of longitudinal hospital records and 28 data modalities. Labs, notes, pathology images, medications, diagnoses — all unified into a single representation. What APOLLO produces is what the authors call a "virtual patient" — a computable embedding that captures not just the current clinical state, but the full trajectory of how that patient got there.

The implications for risk prediction, treatment response modeling, and clinical trial matching are substantial. This is the foundation model moment that healthcare has been waiting for.

---

## [SECTION 7 — DATA ANALYSIS & PRESENTATIONS] ~1 min

Two tools that deserve explicit mention because they remove traditional barriers.

For data: paste a CSV of patient outcomes into ChatGPT Data Analyst or Claude. Ask for Kaplan-Meier curves, multivariate regression, subgroup analysis. Get publication-ready figures. No statistical software license, no programming background required. For early-stage analysis and hypothesis generation, this is transformative.

For presentations: beyond Kimi, **Gamma** and **Beautiful.ai** generate structured visual presentations from your content. The workflow is: upload your abstract and key figures, describe your audience, get a complete slide deck. For a conference presentation under time pressure, this is a genuine time saver.

**Image generation** for surgical education is also maturing fast. Tools like Gemini 3.1 Flash Image — which went viral under the name Nano Banana 2 — generate anatomical illustrations, surgical diagrams, and educational infographics from text descriptions. Perfect for teaching materials and conference posters.

---

## [SECTION 8 — VOICE AGENTS & CONVERSATIONAL CLINICAL TOOLS] ~1.5 min

I want to close with a category that connects everything we've discussed — and represents where clinical AI is actually going.

Voice AI agents.

I've spent the last year building voice-based clinical tools using open-source frameworks — specifically LiveKit, which provides the real-time communication layer — combined with large language models, speech recognition, and the RAG and RLM architectures we just discussed.

What this looks like in practice: a patient can have a spoken conversation with an AI agent that has access to clinical guidelines, remembers the context of previous sessions, and adapts its responses based on what it's learned across conversations. The agent is persistent — it doesn't forget between sessions. It has what we call a memory architecture: structured recall of clinical facts layered with semantic search across the full history.

We built this for goals-of-care conversations — patients with serious illness, discussing their preferences for end-of-life care. The AI agent — we call her Grace — can explain what a DNR means, what POLST forms are, what palliative care involves, and adapt those explanations to a 45-year-old pilot's concerns versus a 78-year-old patient's entirely different set of questions.

Closer to home — for this audience — we built a conversational risk assessment system for cardiac surgery. The AATS AQG calculator you may know as a web form. We rebuilt it as a natural language interface. A clinician describes a patient: "65-year-old male, CABG, history of diabetes, transfer with prolonged pre-op stay." The AI extracts the variables, makes reasonable assumptions for missing data, and returns risk predictions for operative mortality, stroke, renal failure, and six other endpoints — instantly, conversationally, with what-if scenario comparison. No form filling.

The combination of voice, persistent memory, and clinical knowledge bases is producing tools that feel qualitatively different from anything that existed three years ago.

---

## [SECTION 9 — WHAT'S NEXT] ~0.5 min

We're 90 minutes together this morning. Bring your laptop. Try the tools live. Ask questions about your specific problems — clinical, research, administrative, educational.

The AI landscape in 2026 has crossed a threshold. These tools are no longer speculative. They work. The question is whether you'll be the surgeon who uses them, or the surgeon who watches while everyone else does.

I'm looking forward to the conversation.

---

*Total estimated narration time: ~14.5 minutes at comfortable speaking pace*
