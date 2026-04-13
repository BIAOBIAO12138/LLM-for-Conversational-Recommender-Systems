

# Large Language Models for Conversational Recommender Systems

A curated repository for our survey on **LLM-based conversational recommender systems (CRS)**.

This repository contains the manuscript source and a lightweight paper index organized from two complementary perspectives:

- **Application scenarios**: what role LLMs play in CRS
- **Technical paradigms**: how LLMs are integrated into CRS

The survey manuscript source is available in [`main_arxiv.tex`](./main_arxiv.tex).

## Overview

Conversational recommender systems aim to understand user needs through multi-turn interaction and provide grounded, personalized recommendations. With the introduction of large language models, CRS research has rapidly expanded from prompt-based interaction to retrieval grounding, fine-tuning, multi-agent planning, data construction, simulation, and trustworthy deployment.

To make this landscape easier to navigate, we organize the literature in this repository along:

- **6 application scenarios**
- **5 technical paradigms**

This README is intended as a quick entry point for readers, while the full survey provides a more systematic discussion.

## Application Scenarios

| **Scenario** | **Representative papers** | **What LLMs mainly do** |
|---|---|---|
| **User Modeling** | Zero-shot-CRS, MemoCRS, PEBOL, CORAL, UX-LLM-CRS | Infer evolving preferences, maintain memory, capture implicit signals, and model user behavior over multi-turn interaction |
| **Conversation Management** | CP-Rec, InteRecAgent, SAPIENT, MACRS, ECPO | Decide what to ask, when to recommend, how to explain, and how to adapt the dialogue policy from user feedback |
| **External Knowledge Integration** | UniCRS, RecLLM, RA-Rec, CRAG, RAGCRS, STEP | Ground recommendation and explanation in retrieved evidence, knowledge graphs, reviews, and dynamic item information |
| **Data Construction and Augmentation** | LLM-REDIAL, LLM-DA, VCRS, LaViC, DistillRecDial, CeReal | Construct, augment, rewrite, and diversify CRS datasets, including multimodal and persona-aware resources |
| **Evaluation and Benchmarking** | Behavior-Alignment, USCR, PEPPER, CRS-Arena, RecUserSim, UX4CRS | Evaluate interaction quality, benchmark multi-turn behavior, and build user simulators for scalable assessment |
| **Trustworthy Recommendation** | MBRec, TBCRS, PopNudge, crs-fair | Audit and mitigate bias, improve fairness, and analyze safety risks across the conversational lifecycle |

## Technical Paradigms

| **Paradigm** | **Representative papers** | **Core idea** |
|---|---|---|
| **Prompt Engineering** | Zero-shot-CRS, FP-CRS, ILM, PC-CRS, RTA | Control LLM behavior through instructions, templates, and in-context design without heavy training |
| **Soft Prompt Tuning** | UniCRS, CP-Rec, DCRS, ECR, MCKP | Inject task-relevant signals through learnable prompt embeddings while keeping most backbone parameters frozen |
| **Fine-Tuning** | PECRS, LLMCRS, SymRec, ECPO, SumRec-DPO | Adapt model parameters or lightweight modules for stronger personalization, alignment, and domain specialization |
| **Retrieval-Enhanced Methods** | RecLLM, ReFICR, RA-Rec, CRAG, RAGCRS, MOCHA | Ground recommendations with retrieved external evidence such as item metadata, reviews, passages, and graph knowledge |
| **Agent-based Methods** | MACRS, Hybrid-MACRS, InteRecAgent, OMuleT, CRAVE, AdaptJobRec | Turn CRS into a planning-and-tool-use system with explicit role decomposition, workflow coordination, and multi-step decision making |

## Reading Map

If you want a quick reading path through the literature, the following route works well:

1. Start with **User Modeling**, **Conversation Management**, and **External Knowledge Integration** to understand the online CRS pipeline.
2. Then read **Prompt Engineering**, **Fine-Tuning**, and **Retrieval-Enhanced Methods** to see the major implementation routes.
3. Finally, move to **Evaluation**, **Trustworthy Recommendation**, and **Agent-based Methods** for system-level concerns.

## Repository Structure

```text
.
├── README.md
├── main_arxiv.tex
├── sample-base.bib
├── named.bst
├── fig/
└── author/
```

- [`main_arxiv.tex`](./main_arxiv.tex): main survey manuscript
- [`sample-base.bib`](./sample-base.bib): bibliography file
- [`fig/`](./fig): figures used in the manuscript
- [`author/`](./author): author images and related assets

## Citation

If you find this repository helpful, please cite our survey paper.

The manuscript source is currently included in this repository. You can update this section with the final public paper link and BibTeX entry once the paper is released.

## Notes

- This README is a compact index rather than the full survey.
- For full paper titles and bibliographic details, please refer to [`sample-base.bib`](./sample-base.bib).
- The scenario and technique groupings follow the taxonomy used in the survey manuscript.
