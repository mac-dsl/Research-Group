# Database & LLM Research Group

A group space for discussing research at the intersection of databases and large language models. We share papers, give short introductions, and explore ideas together. The topics below are starting points; new directions are welcome.

## Research Topics

| Area | Topics for discussion |
| --- | --- |
| **Data management for pretraining** | Data curation, quality control, deduplication, and training data selection |
| **Fine-tuning and adaptation** | Supervised fine-tuning (SFT), instruction data generation, human-in-the-loop learning, and parameter-efficient fine-tuning (LoRA/PEFT) |
| **Retrieval-Augmented Generation (RAG)** | Data discovery and integration, chunking, hybrid search, reranking, evidence relevance and sufficiency, noise robustness, and provenance |
| **Tabular RAG and table reasoning** | Retrieval over tables and text, table pruning, SQL-based execution, and data quality for analytical questions |
| **Vector databases and Approximate Nearest Neighbor (ANN) search** | Index design, recall–latency trade-offs, filtered search, compression, dynamic updates, and scalable search |
| **Text-to-SQL** | Schema linking, join-path selection, ambiguity resolution, and SQL correctness verification |

## Paper Reading List

Starting papers introduced in the [2026-09-15 group meeting](slides/2026-09-15-intro.pdf). Members are welcome to add papers from these or other research areas.

| Topic | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Instruction tuning | Self-Instruct: Aligning Language Models with Self-Generated Instructions | ACL | 2023 | [Paper](https://aclanthology.org/2023.acl-long.754/) · [PDF](https://aclanthology.org/2023.acl-long.754.pdf) |
| Tabular RAG | TableRAG: A Retrieval Augmented Generation Framework for Heterogeneous Document Reasoning | EMNLP | 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.710/) · [PDF](https://aclanthology.org/2025.emnlp-main.710.pdf) |
| TableQA / denoising | When TableQA Meets Noise: A Dual Denoising Framework for Complex Questions and Large-scale Tables (EnoTab) | ACL | 2026 | [Paper](https://aclanthology.org/2026.acl-long.1102/) · [PDF](https://aclanthology.org/2026.acl-long.1102.pdf) |
| RAG for small models | DRAG: Distilling RAG for SLMs from LLMs to Transfer Knowledge and Mitigate Hallucination via Evidence and Graph-based Distillation | ACL | 2025 | [Paper](https://aclanthology.org/2025.acl-long.358/) · [PDF](https://aclanthology.org/2025.acl-long.358.pdf) |
| Robust RAG / preference optimization | RoseRAG: Robust Retrieval-augmented Generation with Small-scale LLMs via Margin-aware Preference Optimization | Findings of ACL | 2025 | [Paper](https://aclanthology.org/2025.findings-acl.676/) · [PDF](https://aclanthology.org/2025.findings-acl.676.pdf) |

## Group Meetings & Slides

| Date | Presentation | Presenter | Slides |
| --- | --- | --- | --- |
| 2026-09-15 | Database for LLM — Research Overview | Jongjun Park | [PDF](slides/2026-09-15-intro.pdf) |

## Join the Discussion

- Suggest a topic or paper through an [issue](https://github.com/mac-dsl/Research-Group/issues) or a pull request.
- Add papers to the table with their topic, title, venue, year, and source link.
- For a meeting, bring a short introduction, a few questions, or an idea to discuss. A full presentation is optional.
- Upload presentation PDFs to `slides/` using `YYYY-MM-DD-short-title.pdf`, and add a row to the meeting table.

## Repository Structure

```text
README.md                       # Research topics, reading list, and meetings
slides/
    2026-09-15-intro.pdf         # Introductory group presentation
```
