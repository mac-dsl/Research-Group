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
| **Data quality and cleaning** | Error detection and repair, retrieval-based cleaning, and task-aware cleaning recommendations. |
| **LLM-based data processing** | Semantic operators, declarative data processing, query optimization, and accuracy–cost trade-offs. |

## Paper Reading List

Papers for group reading and discussion, including the starting papers introduced in the [2026-09-15 group meeting](slides/2026-09-15-intro.pdf).

The list uses two levels: **Area → Category**. Area headings follow Research Topics above; categories group papers by a shared research focus, rather than by a particular paper or method. Category names and boundaries can be revised as the reading list grows. Each paper is listed once under its primary discussion area. Venue and year refer to the linked publication; preprints are labeled explicitly.

### Data management for pretraining

- **Training Data Curation:** Dataset construction, filtering, deduplication, selection, and mixing for pretraining.
- **Data Management Foundations:** Surveys and perspectives on data management across the model lifecycle, including pretraining, adaptation, and inference.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Training Data Curation | DataComp-LM: In search of the next generation of training sets for language models | NeurIPS (Datasets and Benchmarks) | 2024 | [Paper](https://proceedings.nips.cc/paper_files/paper/2024/hash/19e4ea30dded58259665db375885e412-Abstract-Datasets_and_Benchmarks_Track.html) |
| Data Management Foundations | Data Management For Training Large Language Models: A Survey | arXiv (preprint) | 2023 | [Paper](https://arxiv.org/abs/2312.01700) |
| Data Management Foundations | Position Paper: Data-Centric AI in the Age of Large Language Models | Findings of EMNLP | 2024 | [Paper](https://aclanthology.org/2024.findings-emnlp.695/) · [PDF](https://aclanthology.org/2024.findings-emnlp.695.pdf) |

### Fine-tuning and adaptation

**Instruction Tuning:** Papers on instruction-following adaptation and the generation, selection, or use of instruction data.

**Human Feedback and Alignment:** Learning from human demonstrations, preferences, and reward signals to align model behavior.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Instruction Tuning | Self-Instruct: Aligning Language Models with Self-Generated Instructions | ACL | 2023 | [Paper](https://aclanthology.org/2023.acl-long.754/) · [PDF](https://aclanthology.org/2023.acl-long.754.pdf) |
| Instruction Tuning | LIMA: Less Is More for Alignment | NeurIPS | 2023 | [Paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/ac662d74829e4407ce1d126477f4a03a-Abstract-Conference.html) |
| Instruction Tuning | A Survey on Data Selection for LLM Instruction Tuning | JAIR | 2025 | [Paper](https://doi.org/10.1613/jair.1.17625) · [Preprint PDF](https://arxiv.org/pdf/2402.05123) |
| Human Feedback and Alignment | Training language models to follow instructions with human feedback | NeurIPS | 2022 | [Paper](https://proceedings.neurips.cc/paper/2022/hash/b1efde53be364a73914f58805a001731-Abstract-Conference.html) |

### Retrieval-Augmented Generation (RAG)

- **Tabular RAG:** Papers on retrieval and evidence preparation for answering questions over tabular data, including table selection, pruning, and reasoning over tables and text. Related TableQA and multi-table retrieval methods such as EnoTab and GRIT are included here for comparison.
- **RAG for Small Language Models:** Papers on adapting RAG to small language models, including distillation, training, and retrieval or context design.

- **RAG Foundations:** Core retrieval–generation architectures and learning methods.
- **Table Discovery:** Finding relevant tables in data lakes; these methods support retrieval without necessarily implementing a full RAG pipeline.
- **Retrieval and Search Agents:** Learning retrieval policies and multi-step search strategies.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Tabular RAG | TableRAG: A Retrieval Augmented Generation Framework for Heterogeneous Document Reasoning | EMNLP | 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.710/) · [PDF](https://aclanthology.org/2025.emnlp-main.710.pdf) |
| Tabular RAG | When TableQA Meets Noise: A Dual Denoising Framework for Complex Questions and Large-scale Tables (EnoTab) | ACL | 2026 | [Paper](https://aclanthology.org/2026.acl-long.1102/) · [PDF](https://aclanthology.org/2026.acl-long.1102.pdf) |
| Tabular RAG | GRIT: Guided Relational Integration for Efficient Multi-Table Understanding | EMNLP | 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.1118/) · [PDF](https://aclanthology.org/2025.emnlp-main.1118.pdf) |
| RAG for Small Language Models | DRAG: Distilling RAG for SLMs from LLMs to Transfer Knowledge and Mitigate Hallucination via Evidence and Graph-based Distillation | ACL | 2025 | [Paper](https://aclanthology.org/2025.acl-long.358/) · [PDF](https://aclanthology.org/2025.acl-long.358.pdf) |
| RAG for Small Language Models | RoseRAG: Robust Retrieval-augmented Generation with Small-scale LLMs via Margin-aware Preference Optimization | Findings of ACL | 2025 | [Paper](https://aclanthology.org/2025.findings-acl.676/) · [PDF](https://aclanthology.org/2025.findings-acl.676.pdf) |
| RAG for Small Language Models | MiniRAG: A Lightweight RAG system with Small Language Models | ACL | 2026 | [Paper](https://aclanthology.org/2026.acl-long.1721/) · [PDF](https://aclanthology.org/2026.acl-long.1721.pdf) |
| RAG Foundations | Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks | NeurIPS | 2020 | [Paper](https://proceedings.neurips.cc/paper/2020/file/6b493230205f780e1bc26945df7481e5-Paper.pdf) |
| Table Discovery | Fantastic Tables and Where to Find Them: Table Search in Semantic Data Lakes | EDBT | 2025 | [Paper](https://www.openproceedings.org/2025/conf/edbt/paper-108.pdf) |
| Retrieval and Search Agents | s3: You Don’t Need That Much Data to Train a Search Agent via RL | EMNLP | 2025 | [Paper](https://aclanthology.org/2025.emnlp-main.1095/) · [PDF](https://aclanthology.org/2025.emnlp-main.1095.pdf) |

### Vector databases and Approximate Nearest Neighbor (ANN) search

No papers listed yet. Add a category with the first paper.

### Text-to-SQL

**Benchmarks and Evaluation:** Datasets, evaluation protocols, and comparative studies of natural-language-to-SQL systems.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Benchmarks and Evaluation | Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task | EMNLP | 2018 | [Paper](https://aclanthology.org/D18-1425/) · [PDF](https://aclanthology.org/D18-1425.pdf) |
| Benchmarks and Evaluation | Text-to-SQL Empowered by Large Language Models: A Benchmark Evaluation | PVLDB | 2024 | [Paper](https://www.vldb.org/pvldb/vol17/p1132-gao.pdf) |

### Data quality and cleaning

- **LLM-Assisted Data Cleaning:** Using LLMs and retrieved evidence to detect or repair data errors.
- **Task-Aware Data Cleaning:** Selecting cleaning actions based on downstream task utility, including related ML methods.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| LLM-Assisted Data Cleaning | RetClean: Retrieval-Based Data Cleaning Using LLMs and Data Lakes | PVLDB (Demo) | 2024 | [Paper](https://www.vldb.org/pvldb/vol17/p4421-eltabakh.pdf) |
| LLM-Assisted Data Cleaning | GIDCL: A Graph-Enhanced Interpretable Data Cleaning Framework with Large Language Models | PACMMOD (SIGMOD) | 2024 | [Paper](https://doi.org/10.1145/3698811) · [PDF](https://authurlord.github.io/files/Conference/GIDCL-SIGMOD25.pdf) |
| Task-Aware Data Cleaning | Step-by-Step Data Cleaning Recommendations to Improve ML Prediction Accuracy | EDBT | 2025 | [Paper](https://www.openproceedings.org/2025/conf/edbt/paper-152.pdf) |

### LLM-based data processing

**Semantic Operators and Optimization:** LLM-powered data operators and their execution strategies, costs, and accuracy guarantees.

| Category | Paper | Venue | Year | Links |
| --- | --- | --- | --- | --- |
| Semantic Operators and Optimization | Semantic Operators and Their Optimization: Enabling LLM-Based Data Processing with Accuracy Guarantees in LOTUS | PVLDB | 2025 | [Paper](https://www.vldb.org/pvldb/vol18/p4171-patel.pdf) |

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
