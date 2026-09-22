# Dave Pollack

**Product & design strategy · AI product · research-led evaluation**

Chicago, IL · [davidjpollack.com](https://davidjpollack.com) · [LinkedIn](https://www.linkedin.com/in/dave-pollack)

---

I build AI products and the evaluation programs that decide whether they're safe to ship. The method is UX research discipline applied to systems that talk back: read the outputs before naming anything, define every category so a second person could apply it, and write down the limits next to the numbers.

As founder of **Prox**, I took a RAG-based discovery platform to production — Voyage AI embeddings, pgvector, Claude, a 300K+ product search surface, live Stripe billing. The part I'm proudest of is the evaluation program underneath it: a hand-built failure taxonomy, a four-dimension rubric, a reproducibility-locked LLM-as-judge, and pre-committed ship/hold gates I ran against my own work. One gate returned HOLD on a prompt redesign I'd built. I retired it, fixed the retrieval bug the same run exposed, and re-gated clean.

Before Prox: discovery and evaluative research into shipped features at Capital One Travel, and product discovery at EY (Barclays, Morgan Stanley, Pfizer) and Prudential. MBA and Master of Design.

## How I build

I work through AI-assisted development. Claude writes most of the code; I own what makes it a product — the product decisions, the architecture and vendor choices, the evaluation design, and the release gating. Evaluation is where I've gone deepest, and it's the through-line of everything below.

## What's here

| Repo | What it shows |
|---|---|
| [llm-failure-taxonomy](https://github.com/D-Pollack/llm-failure-taxonomy) | A 25-tag failure taxonomy for Prox's chat assistant, built from 163 hand-labeled failures. Includes the labeled data, the scoring rubrics, the judge prompt, and a dependency-free script that recounts every headline number. |
| [rag-architecture](https://github.com/D-Pollack/rag-architecture) | How the production RAG system works: retrieval cascade, deterministic fusion, generation, and where the evaluation program instruments it. |

The Prox product itself is closed-source. These repos are the sanitized public side of how it was built and verified — redacted of partner, catalog and infrastructure detail, with the data unedited.

**A finding worth the click:** 116 of 163 failures (71%) originated at one pipeline step — the point where the model turns a user's message into structured search inputs. Not the generator, and not retrieval. `node tally.mjs` recounts it from the labeled data in about a second.

**A judgment call worth the click:** across three identical runs, a newer and more capable model flipped 17% of its own factuality pass/fail verdicts (13 of 76). A baseline you can't re-measure isn't a baseline, so the judge is the older model, pinned at temperature 0 with a locked rubric.

## Currently

Open to **AI Product Manager**, **AI Enablement**, and research-led product roles — remote or Chicago hybrid. The pitch: build-and-verify rigor for a team shipping AI features.

📫 dpollack.j@gmail.com
