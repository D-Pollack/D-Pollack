# Dave Pollack

**AI Product & Platform Manager · RAG & LLM Evaluation Systems · Product Strategy & Delivery**

Chicago, IL · [LinkedIn](https://www.linkedin.com/in/dave-pollack) · [proxdesign.co](https://www.proxdesign.co)

---

I build AI products that ship — and I build the evaluation systems that prove they're safe to ship.

As founder of **Prox**, I took a RAG-based AI discovery platform to production: Voyage AI embeddings, pgvector, Claude, 300K+ products, live Stripe billing. The part I'm proudest of is the evaluation program underneath it — a hand-calibrated 4-dimension rubric, a reproducibility-locked LLM-as-judge, and pre-committed ship/hold gates that I ran against my own features. One gate returned HOLD on a prompt redesign I'd built; I retired it, fixed the retrieval bug the same run surfaced, and re-gated clean.

Before Prox: drove discovery and evaluative research into shipped features at Capital One Travel, and led product discovery at EY (Barclays, Morgan Stanley, Pfizer), and Prudential. MBA + Master of Design.

## How I build

I work through AI-assisted development — Claude writes most of the code, and I own everything that makes it a product: product decisions, architecture choices, model and vendor evaluation, and release gating. This soloprenuer model has been my entry point into the world of AI. Through this endeavor, I found that evaluation design and implementation is the area that I focus on the most. 

The evaluation program is where verification rigor lives, and it's the through-line of everything pinned below.

## What's here

| Repo | What it shows |
|---|---|
| [llm-eval-program](https://github.com/D-Pollack/llm-eval-program) | The full LLM evaluation methodology I run at Prox — rubrics, judge calibration, failure taxonomy, dataset lifecycle, ship/hold gates — plus the dataset-integrity tooling from CI |
| [prox-decision-records](https://github.com/D-Pollack/prox-decision-records) | Decision records from building Prox: model selection, retrieval migration, release governance, build-vs-buy |
| [prox-rag-architecture](https://github.com/D-Pollack/prox-rag-architecture) | Architecture writeup of the production RAG system — retrieval cascade, fusion, generation, and how the eval program instruments it |

The Prox product itself is closed-source (it's a live commercial system); these repos are the sanitized, public side of how it was built and verified.

## Currently

Open to **AI Product Manager**, **AI Enablement**, and select AI-focused **UX Research** roles — remote or Chicago hybrid. The pitch: build-and-verify rigor for an established product team working on AI/GenAI.

📫 dpollack.j@gmail.com
