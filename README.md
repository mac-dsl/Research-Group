# Database & LLM Research Group

A group space for discussing research at the intersection of databases and large language models. We share papers, give short introductions, and explore ideas together. The topics below are starting points; new directions are welcome.

## Research Topics

| Area | Topics for discussion |
| --- | --- |
| **Data management for pretraining** | Data curation, quality control, deduplication, and training data selection |
| **Fine-tuning and adaptation** | Supervised fine-tuning (SFT), instruction data generation, human-in-the-loop learning, and parameter-efficient fine-tuning (LoRA/PEFT) |
| **Retrieval-Augmented Generation (RAG)** | Data discovery and integration, chunking, hybrid search, reranking, evidence relevance and sufficiency, noise robustness, provenance, tabular retrieval and reasoning, and RAG for small language models |
| **Vector databases and Approximate Nearest Neighbor (ANN) search** | Index design, recall–latency trade-offs, filtered search, compression, dynamic updates, and scalable search |
| **Text-to-SQL** | Schema linking, join-path selection, ambiguity resolution, and SQL correctness verification |

## Paper Reading List

Starting papers introduced in the [2026-09-15 group meeting](slides/2026-09-15-intro.pdf).

The list uses two levels: **Area → Category**. Area headings follow Research Topics above; categories group papers by a shared research focus, rather than by a particular paper or method. Category names and boundaries can be revised as the reading list grows.

### Data management for pretraining

No papers listed yet. Add a category with the first paper.

### Fine-tuning and adaptation

**Instruction Tuning:** Papers on instruction-following adaptation and the generation, selection, or use of instruction data.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Instruction Tuning | Self-Instruct: Aligning Language Models with Self-Generated Instructions | ACL | 2023 | [Paper](https://aclanthology.org/2023.acl-long.754/) · [PDF](https://aclanthology.org/2023.acl-long.754.pdf) |

### Retrieval-Augmented Generation (RAG)

- **Tabular RAG:** Papers on retrieval and evidence preparation for answering questions over tabular data, including table selection, pruning, and reasoning over tables and text. Related TableQA methods such as EnoTab are included here for comparison.
- **RAG for Small Language Models:** Papers on adapting RAG to small language models, including distillation, training, and retrieval or context design.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Tabular RAG | TableRAG: A Retrieval Augmented Generation Framework for Heterogeneous Document Reasoning | EMNLP | 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.710/) · [PDF](https://aclanthology.org/2025.emnlp-main.710.pdf) |
| Tabular RAG | When TableQA Meets Noise: A Dual Denoising Framework for Complex Questions and Large-scale Tables (EnoTab) | ACL | 2026 | [Paper](https://aclanthology.org/2026.acl-long.1102/) · [PDF](https://aclanthology.org/2026.acl-long.1102.pdf) |
| RAG for Small Language Models | DRAG: Distilling RAG for SLMs from LLMs to Transfer Knowledge and Mitigate Hallucination via Evidence and Graph-based Distillation | ACL | 2025 | [Paper](https://aclanthology.org/2025.acl-long.358/) · [PDF](https://aclanthology.org/2025.acl-long.358.pdf) |
| RAG for Small Language Models | RoseRAG: Robust Retrieval-augmented Generation with Small-scale LLMs via Margin-aware Preference Optimization | Findings of ACL | 2025 | [Paper](https://aclanthology.org/2025.findings-acl.676/) · [PDF](https://aclanthology.org/2025.findings-acl.676.pdf) |

### Vector databases and Approximate Nearest Neighbor (ANN) search

No papers listed yet. Add a category with the first paper.

### Text-to-SQL

No papers listed yet. Add a category with the first paper.

## Group Meetings & Slides

| Date | Presentation | Presenter | Slides |
| --- | --- | --- | --- |
| 2026-09-15 | Database for LLM — Research Overview | Jongjun Park | [PDF](slides/2026-09-15-intro.pdf) |

## Join the Discussion

- Suggest a topic or paper through an [issue](https://github.com/mac-dsl/Research-Group/issues) or a pull request.
- Add each paper under the appropriate Area with its category, title, venue, year, and source link. Reuse an existing category when it fits; propose or revise a category when needed.
- For a meeting, bring a short introduction, a few questions, or an idea to discuss. A full presentation is optional.
- Upload presentation PDFs to `slides/` using `YYYY-MM-DD-short-title.pdf`, and add a row to the meeting table.

## Repository Structure

```text
README.md                       # Research topics, reading list, and meetings
slides/
    2026-09-15-intro.pdf         # Introductory group presentation
```
