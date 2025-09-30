Evaluating Synthetic Data for Pharmacovigilance

This project builds an LLM-driven pipeline for generating and evaluating synthetic social media data on adverse drug events (ADEs). The goal: augment scarce training data for pharmacovigilance models with realistic, diverse synthetic samples.

Engineering Highlights: 

Data Pipeline: Ingested SMM4H annotated tweets (1,824 samples), integrated ChromaDB for context retrieval, and automated zero-shot / one-shot prompting with GPT-4.

Evaluation Framework: Implemented semantic similarity metrics (SentenceTransformers + cosine distance, variance, kurtosis) for dataset diversity benchmarking.

Experimentation: Compared zero-shot, sampled one-shot, and selected one-shot prompting, with reproducible configs (temperature, token limits, seeding).

Modular Codebase: Scripts + notebooks organized for re-runs, scaling, and extensions (e.g., Wasserstein distance, ADE–drug relationship checks).

Key Results: 

One-shot methods generated more diverse datasets than zero-shot.

Sampled one-shot prompting produced the highest variance, confirming hypothesis.

Highlighted trade-off: diversity ≠ quality, motivating richer evaluation metrics.

Future Work

Extend evaluation with Wasserstein distance and ADE–drug relationship fidelity.

Fine-tune extraction models using synthetic data across forums, Reddit, and Twitter.
