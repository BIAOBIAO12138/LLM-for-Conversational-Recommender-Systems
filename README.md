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

The following tables list the methods covered in our survey taxonomy under the five core technical paradigms.

- Total indexed methods in this section: **57**
- Link policy: we use direct arXiv links when they are available in the bibliography; otherwise we provide a Google Scholar search link for quick access.

### Prompt Engineering

| Method | Paper | Venue | Notable Techniques |
|---|---|---|---|
| **Zero-shot CRS** | [Large Language Models as Zero-Shot Conversational Recommenders](https://scholar.google.com/scholar?q=Large%20Language%20Models%20as%20Zero-Shot%20Conversational%20Recommenders) | CIKM 2023 | Zero-shot Prompting |
| **PopNudge** | [Improving Conversational Recommendation Systems via Bias Analysis and Language-Model-Enhanced Data Augmentation](https://scholar.google.com/scholar?q=Improving%20Conversational%20Recommendation%20Systems%20via%20Bias%20Analysis%20and%20Language-Model-Enhanced%20Data%20Augmentation) | EMNLP 2023 | Bias-aware Augmentation |
| **VCRS** | [Towards Building Voice-based Conversational Recommender Systems: Datasets, Potential Solutions and Prospects](https://scholar.google.com/scholar?q=Towards%20Building%20Voice-based%20Conversational%20Recommender%20Systems%3A%20Datasets%2C%20Potential%20Solutions%20and%20Prospects) | SIGIR 2023 | Speech-Attribute Fusion |
| **PC-CRS** | [Beyond Persuasion: Towards Conversational Recommender System with Credible Explanations](https://scholar.google.com/scholar?q=Beyond%20Persuasion%3A%20Towards%20Conversational%20Recommender%20System%20with%20Credible%20Explanations) | EMNLP 2024 | Controlled Prompting, CoT |
| **MemoCRS** | [MemoCRS: Memory-enhanced Sequential Conversational Recommender Systems with Large Language Models](https://scholar.google.com/scholar?q=MemoCRS%3A%20Memory-enhanced%20Sequential%20Conversational%20Recommender%20Systems%20with%20Large%20Language%20Models) | CIKM 2024 | Memory-Augmented |
| **LLM-REDIAL** | [LLM-REDIAL: A Large-Scale Dataset for Conversational Recommender Systems Created from User Behaviors with LLMs](https://scholar.google.com/scholar?q=LLM-REDIAL%3A%20A%20Large-Scale%20Dataset%20for%20Conversational%20Recommender%20Systems%20Created%20from%20User%20Behaviors%20with%20LLMs) | ACL 2024 | Behavior-Aligned Data |
| **ILM** | [Item-Language Model for Conversational Recommendation](https://arxiv.org/abs/2406.02844) | arXiv 2024 | External Param. Adapter |
| **Pearl** | [Pearl: A Review-driven Persona-Knowledge Grounded Conversational Recommendation Dataset](https://scholar.google.com/scholar?q=Pearl%3A%20A%20Review-driven%20Persona-Knowledge%20Grounded%20Conversational%20Recommendation%20Dataset) | ACL 2024 | Persona Extraction |
| **FP-CRS** | [A Flash in the Pan: Better Prompting Strategies to Deploy Out-of-the-Box LLMs as Conversational Recommendation Systems](https://scholar.google.com/scholar?q=A%20Flash%20in%20the%20Pan%3A%20Better%20Prompting%20Strategies%20to%20Deploy%20Out-of-the-Box%20LLMs%20as%20Conversational%20Recommendation%20Systems) | COLING 2025 | CoT Prompting |
| **USB-Rec** | [USB-Rec: An Effective Framework for Improving Conversational Recommendation Capability of Large Language Model](https://scholar.google.com/scholar?q=USB-Rec%3A%20An%20Effective%20Framework%20for%20Improving%20Conversational%20Recommendation%20Capability%20of%20Large%20Language%20Model) | RecSys 2025 | User Simulator |
| **RTA** | [Reindex-Then-Adapt: Improving Large Language Models for Conversational Recommendation](https://scholar.google.com/scholar?q=Reindex-Then-Adapt%3A%20Improving%20Large%20Language%20Models%20for%20Conversational%20Recommendation) | WSDM 2025 | External Param. Fine-Tune |
| **Pan-CRS** | [A Flash in the Pan: Better Prompting Strategies to Deploy Out-of-the-Box LLMs as Conversational Recommendation Systems](https://scholar.google.com/scholar?q=A%20Flash%20in%20the%20Pan%3A%20Better%20Prompting%20Strategies%20to%20Deploy%20Out-of-the-Box%20LLMs%20as%20Conversational%20Recommendation%20Systems) | COLING 2025 | Adaptive Prompting |
| **GRSU** | [Search-Based Interaction For Conversation Recommendation via Generative Reward Model Based Simulated User](https://scholar.google.com/scholar?q=Search-Based%20Interaction%20For%20Conversation%20Recommendation%20via%20Generative%20Reward%20Model%20Based%20Simulated%20User) | SIGIR 2025 | Reward-guided Search |

### Soft Prompt Tuning

| Method | Paper | Venue | Notable Techniques |
|---|---|---|---|
| **UniCRS** | [Towards Unified Conversational Recommender Systems via Knowledge-Enhanced Prompt Learning](https://scholar.google.com/scholar?q=Towards%20Unified%20Conversational%20Recommender%20Systems%20via%20Knowledge-Enhanced%20Prompt%20Learning) | KDD 2022 | Unified Prompting |
| **CP-Rec** | [CP-Rec: Contextual prompting for conversational recommender systems](https://scholar.google.com/scholar?q=CP-Rec%3A%20Contextual%20prompting%20for%20conversational%20recommender%20systems) | AAAI 2023 | Prompt Refinement |
| **DCRS** | [Broadening the View: Demonstration-augmented Prompt Learning for Conversational Recommendation](https://scholar.google.com/scholar?q=Broadening%20the%20View%3A%20Demonstration-augmented%20Prompt%20Learning%20for%20Conversational%20Recommendation) | SIGIR 2024 | Example-based Prompting |
| **ECR** | [Towards Empathetic Conversational Recommender Systems](https://scholar.google.com/scholar?q=Towards%20Empathetic%20Conversational%20Recommender%20Systems) | RecSys 2024 | Emotion-Aware |
| **LGCRS** | [LGCRS: LLM-Guided Representation-Enhancing for Conversational Recommender System](https://scholar.google.com/scholar?q=LGCRS%3A%20LLM-Guided%20Representation-Enhancing%20for%20Conversational%20Recommender%20System) | ICANN 2024 | Semantic-CF Alignment |
| **DisenCRS** | [Beyond Whole Dialogue Modeling: Contextual Disentanglement for Conversational Recommendation](https://scholar.google.com/scholar?q=Beyond%20Whole%20Dialogue%20Modeling%3A%20Contextual%20Disentanglement%20for%20Conversational%20Recommendation) | SIGIR 2025 | Context Disentanglement |
| **MSCRS** | [MSCRS: Multi-modal Semantic Graph Prompt Learning Framework for Conversational Recommender Systems](https://scholar.google.com/scholar?q=MSCRS%3A%20Multi-modal%20Semantic%20Graph%20Prompt%20Learning%20Framework%20for%20Conversational%20Recommender%20Systems) | SIGIR 2025 | Multimodal Fusion |
| **MCKP** | [MCKP: Multi-aspect contextual knowledge-enhanced prompting for conversational recommender systems](https://scholar.google.com/scholar?q=MCKP%3A%20Multi-aspect%20contextual%20knowledge-enhanced%20prompting%20for%20conversational%20recommender%20systems) | Inf. Sci. 2025 | Multi-aspect Context Modeling |
| **GeoCRS** | [From Dialogue to Destination: Geography-Aware Large Language Models with Multimodal Fusion for Conversational Recommendation](https://scholar.google.com/scholar?q=From%20Dialogue%20to%20Destination%3A%20Geography-Aware%20Large%20Language%20Models%20with%20Multimodal%20Fusion%20for%20Conversational%20Recommendation) | AAAI 2026 | Geographic Information Fusion |

### Fine-Tuning

| Method | Paper | Venue | Notable Techniques |
|---|---|---|---|
| **LLMCRS** | [A Large Language Model Enhanced Conversational Recommender System](https://arxiv.org/abs/2308.06212) | arXiv 2023 | In-Context Learning, RLPF |
| **PECRS** | [Parameter-Efficient Conversational Recommender System as a Language Processing Task](https://scholar.google.com/scholar?q=Parameter-Efficient%20Conversational%20Recommender%20System%20as%20a%20Language%20Processing%20Task) | EACL 2024 | Adapter-based PEFT |
| **MMCRec** | [MMCRec: Towards Multi-modal Generative AI in Conversational Recommendation](https://scholar.google.com/scholar?q=MMCRec%3A%20Towards%20Multi-modal%20Generative%20AI%20in%20Conversational%20Recommendation) | ECIR 2024 | Multimodal Graph-of-Thought |
| **SymRec** | [Towards Symbiotic Recommendations: Leveraging LLMs for Conversational Recommendation Systems](https://scholar.google.com/scholar?q=Towards%20Symbiotic%20Recommendations%3A%20Leveraging%20LLMs%20for%20Conversational%20Recommendation%20Systems) | RecSys 2024 | Symbiotic Intelligence |
| **LaViC** | [Adapting Large Vision-Language Models to Visually-Aware Conversational Recommendation](https://scholar.google.com/scholar?q=Adapting%20Large%20Vision-Language%20Models%20to%20Visually-Aware%20Conversational%20Recommendation) | KDD 2025 | Visual Knowledge Distillation |
| **OSMVR** | [One-shot Multi-view Visual Conversational Recommendation](https://scholar.google.com/scholar?q=One-shot%20Multi-view%20Visual%20Conversational%20Recommendation) | KDD 2025 | One-shot Learning |
| **ECPO** | [Expectation Confirmation Preference Optimization for Multi-Turn Conversational Recommendation Agent](https://scholar.google.com/scholar?q=Expectation%20Confirmation%20Preference%20Optimization%20for%20Multi-Turn%20Conversational%20Recommendation%20Agent) | ACL 2025 | Expectation Confirmation, DPO |
| **LLM-DA** | [Beyond Single Labels: Improving Conversational Recommendation through LLM-Powered Data Augmentation](https://scholar.google.com/scholar?q=Beyond%20Single%20Labels%3A%20Improving%20Conversational%20Recommendation%20through%20LLM-Powered%20Data%20Augmentation) | ACL 2025 | Data Augmentation |
| **BRICR** | [Bridging context and knowledge graph: A semantic-enhanced framework for conversational recommendation systems](https://scholar.google.com/scholar?q=Bridging%20context%20and%20knowledge%20graph%3A%20A%20semantic-enhanced%20framework%20for%20conversational%20recommendation%20systems) | KBS 2025 | Cross-distribution Adapter |
| **SumRec-DPO** | [Refining Text Generation for Realistic Conversational Recommendation via Direct Preference Optimization](https://scholar.google.com/scholar?q=Refining%20Text%20Generation%20for%20Realistic%20Conversational%20Recommendation%20via%20Direct%20Preference%20Optimization) | EMNLP 2025 | Direct Preference Optimization |
| **Causal-LLM-CRS** | [Do Mentioned Items Truly Matter? Enhancing Conversational Recommender Systems with Causal Intervention and Large Language Models](https://scholar.google.com/scholar?q=Do%20Mentioned%20Items%20Truly%20Matter%3F%20Enhancing%20Conversational%20Recommender%20Systems%20with%20Causal%20Intervention%20and%20Large%20Language%20Models) | IJCAI 2025 | Confounder Disentanglement |
| **REGEN** | [Beyond Retrieval: Generating Narratives in Conversational Recommender Systems](https://scholar.google.com/scholar?q=Beyond%20Retrieval%3A%20Generating%20Narratives%20in%20Conversational%20Recommender%20Systems) | WWW 2025 | Content Embedding Fusion |
| **Gemma3-Chase** | [A Neuro-Symbolic AI Approach for a Conversational Workout Plan Recommender System](https://scholar.google.com/scholar?q=A%20Neuro-Symbolic%20AI%20Approach%20for%20a%20Conversational%20Workout%20Plan%20Recommender%20System) | iJOE 2026 | Rule-based Reasoning Traces |
| **STARCRS** | [Integrating Vision-Centric Text Understanding for Conversational Recommender Systems](https://scholar.google.com/scholar?q=Integrating%20Vision-Centric%20Text%20Understanding%20for%20Conversational%20Recommender%20Systems) | arXiv 2026 | Visual-token Encoding |

### Retrieval Enhanced

| Method | Paper | Venue | Notable Techniques |
|---|---|---|---|
| **RecLLM** | [Leveraging Large Language Models in Conversational Recommender Systems](https://arxiv.org/abs/2305.07961) | arXiv 2023 | Retrieval-Augmented Tool Use |
| **CRS-LLM** | [Conversational Recommender System and Large Language Model Are Made for Each Other in E-commerce Pre-sales Dialogue](https://scholar.google.com/scholar?q=Conversational%20Recommender%20System%20and%20Large%20Language%20Model%20Are%20Made%20for%20Each%20Other%20in%20E-commerce%20Pre-sales%20Dialogue) | EMNLP 2023 | Bidirectional Collaboration |
| **RA-Rec** | [Retrieval-Augmented Conversational Recommendation with Prompt-based Semi-Structured Natural Language State Tracking](https://scholar.google.com/scholar?q=Retrieval-Augmented%20Conversational%20Recommendation%20with%20Prompt-based%20Semi-Structured%20Natural%20Language%20State%20Tracking) | SIGIR 2024 | RAG, State Tracking |
| **ReFICR** | [Unleashing the Retrieval Potential of Large Language Models in Conversational Recommender Systems](https://scholar.google.com/scholar?q=Unleashing%20the%20Retrieval%20Potential%20of%20Large%20Language%20Models%20in%20Conversational%20Recommender%20Systems) | RecSys 2024 | Instruction Tuning, PEFT |
| **ChatCRS** | [ChatCRS: Incorporating External Knowledge and Goal Guidance for LLM-based Conversational Recommender Systems](https://scholar.google.com/scholar?q=ChatCRS%3A%20Incorporating%20External%20Knowledge%20and%20Goal%20Guidance%20for%20LLM-based%20Conversational%20Recommender%20Systems) | NAACL 2025 | Goal-guided |
| **CRAG** | [Collaborative Retrieval for Large Language Model-based Conversational Recommender Systems](https://scholar.google.com/scholar?q=Collaborative%20Retrieval%20for%20Large%20Language%20Model-based%20Conversational%20Recommender%20Systems) | WWW 2025 | Collaborative Retrieval |
| **G-CRS** | [Graph Retrieval-Augmented LLM for Conversational Recommendation Systems](https://scholar.google.com/scholar?q=Graph%20Retrieval-Augmented%20LLM%20for%20Conversational%20Recommendation%20Systems) | PAKDD 2025 | Graph RAG |
| **COMPASS** | [Reasoning Over User Preferences: Knowledge Graph-Augmented LLMs for Explainable Conversational Recommendations](https://scholar.google.com/scholar?q=Reasoning%20Over%20User%20Preferences%3A%20Knowledge%20Graph-Augmented%20LLMs%20for%20Explainable%20Conversational%20Recommendations) | ICDM 2025 | Knowledge Retrieval |
| **STEP** | [STEP: Stepwise Curriculum Learning for Context-Knowledge Fusion in Conversational Recommendation](https://scholar.google.com/scholar?q=STEP%3A%20Stepwise%20Curriculum%20Learning%20for%20Context-Knowledge%20Fusion%20in%20Conversational%20Recommendation) | CIKM 2025 | Curriculum Learning |
| **CORAL** | [Empowering Retrieval-based Conversational Recommendation with Contrasting User Preferences](https://scholar.google.com/scholar?q=Empowering%20Retrieval-based%20Conversational%20Recommendation%20with%20Contrasting%20User%20Preferences) | NAACL 2025 | Preference Expansion |
| **ESPRESSO** | [ESPRESSO: An Effective Approach to Passage Retrieval for High-Quality Conversational Recommender Systems](https://scholar.google.com/scholar?q=ESPRESSO%3A%20An%20Effective%20Approach%20to%20Passage%20Retrieval%20for%20High-Quality%20Conversational%20Recommender%20Systems) | AAAI 2025 | Adaptive Item Selection |
| **RAGCRS** | [Towards Retrieval-Augmented Large Language Model-Based Conversational Recommender System](https://scholar.google.com/scholar?q=Towards%20Retrieval-Augmented%20Large%20Language%20Model-Based%20Conversational%20Recommender%20System) | PAKDD 2025 | Compare-then-Summarize |
| **MOCHA** | [Leveraging Retrieval-Augmented Language Models for Accurate Item/Feature Selection in Conversational Recommender Systems](https://scholar.google.com/scholar?q=Leveraging%20Retrieval-Augmented%20Language%20Models%20for%20Accurate%20Item/Feature%20Selection%20in%20Conversational%20Recommender%20Systems) | WSDM 2026 | Feature Selection |

### Agent-based

| Method | Paper | Venue | Notable Techniques |
|---|---|---|---|
| **MACRS** | [A Multi-Agent Conversational Recommender System](https://arxiv.org/abs/2402.01135) | arXiv 2024 | Multi-Agent Act Planning |
| **Hybrid-MACRS** | [A Hybrid Multi-Agent Conversational Recommender System with LLM and Search Engine in E-commerce](https://scholar.google.com/scholar?q=A%20Hybrid%20Multi-Agent%20Conversational%20Recommender%20System%20with%20LLM%20and%20Search%20Engine%20in%20E-commerce) | RecSys 2024 | Multi-agent Collaboration |
| **InteRecAgent** | [Recommender AI Agent: Integrating Large Language Models for Interactive Recommendations](https://scholar.google.com/scholar?q=Recommender%20AI%20Agent%3A%20Integrating%20Large%20Language%20Models%20for%20Interactive%20Recommendations) | TOIS 2025 | Agentic Planning, Tool Use |
| **OMuleT** | [OMuleT: Orchestrating Multiple Tools for Practicable Conversational Recommendation](https://arxiv.org/abs/2411.19352) | arXiv 2025 | Multi-Tool Orchestration |
| **CRAVE** | [LLM-based Conversational Recommendation Agents with Collaborative Verbalized Experience](https://scholar.google.com/scholar?q=LLM-based%20Conversational%20Recommendation%20Agents%20with%20Collaborative%20Verbalized%20Experience) | EMNLP 2025 | Debater-Critic Agents |
| **FuseRec** | [Fusing sequential recommender and ad-hoc planner for multi-faceted preference understanding in conversational recommendation](https://scholar.google.com/scholar?q=Fusing%20sequential%20recommender%20and%20ad-hoc%20planner%20for%20multi-faceted%20preference%20understanding%20in%20conversational%20recommendation) | Inf. Fusion 2026 | Multi-faceted Preference Model |
| **AdaptJobRec** | [AdaptJobRec: Enhancing Conversational Career Recommendation through an LLM-Powered Agentic System](https://scholar.google.com/scholar?q=AdaptJobRec%3A%20Enhancing%20Conversational%20Career%20Recommendation%20through%20an%20LLM-Powered%20Agentic%20System) | AAAI 2026 | Agentic Planning, Tool Use |
| **ImpReSS** | [ImpReSS: Designing and Evaluating a Lightweight Implicit Recommender System in Conversational Support Agents](https://scholar.google.com/scholar?q=ImpReSS%3A%20Designing%20and%20Evaluating%20a%20Lightweight%20Implicit%20Recommender%20System%20in%20Conversational%20Support%20Agents) | IUI 2026 | Implicit recommendation |

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
