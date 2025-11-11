# AI Evolution: From Rules to Agents — Learning Resources for Engineering Teams

**Complete package** teaching the 40-year evolution of AI systems through a single use case: **L1 IT Support for a Banking Data Platform**.  
Includes runnable code, slide decks, visual diagrams, and notebooks.

---

## YouTube Primer
- [AI Agents Explained in 5 mins](https://youtu.be/06aWuBMoxGw)  
- [AI Evolution & Choosing Your GenAI Champion in 8 mins](https://youtu.be/Axp8jFCkiHo)

---

## What is this?
A comprehensive learning package that covers AI development stages from rule-based automation to multi-agent workflows. Everything is connected through one real-world use case so teams can compare approaches directly.

---

## Why this exists
- Working code you can run immediately  
- One use case across all stages for direct comparison  
- Real metrics: latency, cost, coverage, dev time  
- A clear decision framework with trade-offs  
- A 4-week structured learning plan

---

## Delivered artifacts
1. **AI Master Evolution Guide (start here)**  
   - `ai-master-evolution-guide.html`  
   - Overview of all 6 stages: Rule-based, Traditional ML, Prompting (GenAI), RAG, Fine-tuning, Agentic AI.  
   - Includes timeline, architecture diagrams, performance metrics, comparison tables, and a 4-week learning plan.

2. **Agentic Workflows Guide (priority)**  
   - `06-agentic-workflows.html`  
   - Deep dive into multi-agent systems, ADK + Gemini implementation patterns, production considerations, safety, and cost control.


3. **Quick Start (navigation hub)**  
   - `00-QUICK-START.html`

4. **This README**  
   - `README.md`

---

## How to use the resources

### Quick start (30 minutes)
1. Open `00-QUICK-START.html`.  
2. Read the "START HERE" section.  
3. Select a learning path by role.  
4. Follow recommended exercises.

### Deep learning (4 weeks)
- **Week 1 — Foundations**: Study stages 1–2, run rule-based agent, build ML classifier.  
- **Week 2 — GenAI & RAG**: Prompt Gemini, build RAG prototype.  
- **Week 3 — Advanced**: Fine-tuning + comparison with RAG.  
- **Week 4 — Agentic systems**: Build multi-agent workflow using ADK.

---

## Directory structure
```
/
├── 00-QUICK-START.html
├── ai-master-evolution-guide.html
├── 06-agentic-workflows.html
├── README.md
└── code_files/
    └── 01-rule-based/
        ├── rag-implementation-l1-support.ipynb
        ├── agentic-ai-implementation-l1-support.ipynb
        └── README_code.md
```
---

## The 6 Stages of AI Evolution

### 1. Rule-based  
- Deterministic, low latency.  
- Coverage ~20%.

### 2. Traditional ML  
- Pattern learning from labeled data.  
- Coverage ~50%.

### 3. GenAI Prompting  
- Flexible language understanding.  
- Coverage ~50%, may hallucinate.

### 4. RAG  
- Grounded generation using a knowledge base.  
- Coverage ~70%.

### 5. Fine-tuning  
- Consistent, domain-trained language model.  
- Ideal for high-volume use.

### 6. Agentic AI  
- Multi-step reasoning and tool use.  
- Coverage ~70%, with 40%+ auto-resolution potential.

---

## Choosing the right approach (decision matrix)

| Need | Best Choice |
|------|--------------|
| Simple rules, low latency | Rule-based |
| Stable labeled data | ML |
| Flexible NLU, fast prototyping | Prompting |
| Truthful answers with docs | RAG |
| Consistent tone & tasks | Fine-tuning |
| Autonomous workflows | Agentic AI |

---

## Expected outcomes
- Ability to explain, compare, and choose approaches.  
- Ability to design and implement RAG + agent workflows.  
- Understanding cost, latency, governance needs.  
- Building working prototypes end-to-end.

---

## Metrics (example)
| Approach | Coverage | Latency | Dev Time | Cost |
|---------|----------|----------|-----------|--------|
| Rule-based | 20% | <100ms | 2 weeks | $0 |
| Traditional ML | 50% | 200ms | 6 weeks | $500 |
| Prompting | 50% | 2–5s | 2 weeks | $2K–$5K |
| RAG | 70% | 3–6s | 4 weeks | $3K–$6K |
| Fine-tuning | 70% | 1–2s | 6–8 weeks | $1K–$2K |
| Agentic | 70% | 5–15s | 12 weeks | $4K–$8K |

---

## Requirements
- Python 3.8+  
- Google ADK (`pip install google-adk`)  
- Gemini API key  
- Vector DB (ChromaDB or FAISS)

---

## References
- Google ADK: https://ai.google.dev/adk  
- Gemini API: https://ai.google.dev/gemini-api  
- ChromaDB: https://www.trychroma.com/

