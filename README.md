# Chrysanthos Panagakos

**Applied AI · Retrieval · Evaluation · Greek-language NLP**

I build AI systems whose outputs can be inspected and evaluated—not merely generated.

My route into applied AI runs through physics education. For 13 years, I have worked with students to identify where their problem-solving process breaks and what might unblock it. I now bring that perspective to retrieval, structured LLM workflows and evaluation.

## Featured project

### [Greek Physics Diagnostic RAG](https://github.com/chpanagakos/greek-physics-rag)

[Live demo](https://huggingface.co/spaces/chpanagakos/greek-physics-rag) · [Repository](https://github.com/chpanagakos/greek-physics-rag)

[![tests](https://github.com/chpanagakos/greek-physics-rag/actions/workflows/tests.yml/badge.svg)](https://github.com/chpanagakos/greek-physics-rag/actions/workflows/tests.yml)

A Greek-language system for analysing incorrect student solutions to Panhellenic physics problems. It retrieves relevant curriculum material, proposes candidate labels from a tutor-reviewed diagnostic taxonomy, and presents the retrieved passages for human review.

`Surya OCR → BGE-M3 → Qdrant → Gemini → Gradio`

The project includes:

* A resumable ingestion pipeline for Greek scientific documents with mathematical OCR, atomic page-level writes and structure-aware chunking
* Dense multilingual retrieval over worked solutions and theory
* Schema-validated LLM output constrained to a 15-label taxonomy, with an explicit `NO_TAG_MATCH` outcome
* Source identifiers, a visible retrieval audit panel and an in-app retrieval ablation
* A reproducible evaluation harness with manually assigned misconception labels and source-relevance judgements
* Automated tests and continuous integration

On the current 10-case development set, retrieval achieved Recall@5 of **0.80** and MRR of **0.70**; a retrieval ablation produced an identical diagnosis in 9 of 10 cases, with one reproducible correction attributable to a retrieved chunk. The repository documents the evaluation protocol, the retrieval misses and the planned held-out test set.
## Background

* **MSc, Data Science & Machine Learning** — Hellenic Open University, 2025, final grade 9.63/10
* **BSc, Theoretical Physics** — Lancaster University
* **13 years in physics education** — individual and small-group teaching, including preparation for Greece’s Panhellenic university-entrance examinations

## Technical focus

* **Applied AI:** RAG, embeddings, vector search, structured LLM output, OCR and document-processing pipelines
* **Evaluation:** relevance labelling, Recall@k, MRR, ablation studies and reproducible offline scoring
* **Engineering:** Python, SQL, scikit-learn, pytest, GitHub Actions, Linux, Git and shell scripting

## Current direction

I am extending the project with a held-out evaluation set derived from observed student errors, stronger citation-support checks and hybrid dense–sparse retrieval.

I am open to remote and Athens-based Applied AI and ML engineering roles.

## Contact

[Email](mailto:cp@panagakos.dev) · [LinkedIn](https://www.linkedin.com/in/chpanagakos/)
