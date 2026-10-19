# Multimodal LLM Knowledge Extraction & Prompt Evaluation Pipeline

> **Note on Scope**: This is an applied AI research and document-intelligence prototype engineered to clean, ingest, and validate unstructured or degraded physical texts (historical manuscripts, technical reports, invoices) into structured relational schemas for downstream retrieval and analytics.

---

## 1. Project Overview

**Multimodal LLM Knowledge Extraction & Prompt Evaluation Pipeline** (`ocr_updated`) is a robust document-intelligence framework that solves the challenge of extracting structured data from noisy, low-resolution, or degraded document layouts.

The system couples traditional computer vision OCR with modern multimodal large language models and rigorous benchmark evaluation:
- **3-Stage Multimodal Ingestion**: Combines document layout analysis (DocTR, EasyOCR, LayoutLMv3) with **Google Cloud Gemini 2.5 Flash API** to handle visual spatial formatting and textual transcription simultaneously.
- **Structured Prompt Engineering**: Utilizes few-shot prompting, chain-of-thought instructions, and **Pydantic schema validation** to force deterministic JSON/SQL outputs from unstructured text.
- **Forensic Error Analysis & Benchmarking**: Systematic evaluation suite testing 6 Document AI architectures across defined test cases to root-cause hallucinations and formatting drift.
- **Optimized Recall & Precision**: Achieves **97.37% recall**, **95.59% F1-score**, and a **33% reduction in false-positive extractions** (177 $\rightarrow$ 118 errors) while raising precision from **81.6% to 90.2%**.

---

## 2. Architecture Diagram
