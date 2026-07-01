---
title: CareChorus
subtitle: Evaluation Infrastructure for an AI-Powered Healthcare Companion App
summary: AI-driven mobile app for patient care navigation and medical document classification.
featured_image: ''
tags:
  - Dart
  - Flutter
  - Large Language Models
  - LLM Evaluation
  - LLM-as-a-Judge
  - Prompt Engineering
  - Structured Information Extraction
date: 2026-03-01
institution: University of Washington | Seattle, WA
affiliation: University of Washington
start_date: 2026-03-01
end_date: 2026-06-30
---

<video autoplay loop muted playsinline style="width:100%;border-radius:8px;">
  <source src="demo.mp4" type="video/mp4">
</video>

CareChorus is a local-first, Flutter-based healthcare companion app that helps patients and caregivers manage complex medical journeys. Its core AI pipeline ingests uploaded documents and photos (lab reports, discharge summaries, medication labels, imaging results) and runs them through a classify → extract → summarize flow across multiple LLMs (Claude Sonnet 4.5, GPT-5, GPT-5-mini) to populate a schema-driven record of medications, conditions, providers, and appointments — turning dense medical paperwork into structured, actionable data while keeping protected health information on-device. As eval infrastructure lead, I designed and built the testing and quality-assurance systems that validate this pipeline's accuracy before it ships to patients.

## Key Contributions

- Built the document-processing evaluation CLI (`pipeline.dart`, `document_processor.dart`) that replays CareChorus's production classify/extract/summarize flow against a corpus of real-world medical documents to validate output quality before release.
- Implemented an LLM-as-judge quality assessment tool (`judge.dart`) that flags structured extraction gaps — structural omissions, formatting loss, incorrect or missing fields — with severity ratings, turning ad hoc spot-checking into a repeatable, human-reviewable process.
- Authored a ground-truth generation tool (`generate_gt.dart`) that produces independent Markdown transcriptions of source documents using a separate model from the extraction pipeline, enabling apples-to-apples fidelity comparisons.
- Extended the evaluation framework (`carechorus-evals`) into a Promptfoo-based suite of 17 automated assertions covering classification confidence, extraction completeness, date formatting, and summarization quality, achieving a 100% pass rate across a 17-document real-world medical record test set.
- Maintained a standalone legacy evaluation script (`workspace/document_translator.dart`) for offline and CI-driven pipeline validation, kept in sync with production prompt templates by importing them directly from the main app.
- Worked within CareChorus's schema-driven, plugin-extensible intake architecture (15 clinical entity types spanning medications, conditions, providers, and appointments) to ensure evaluation coverage scaled alongside new data types without pipeline rewrites.

## Technologies

**Languages:** Dart

**AI & Machine Learning:** Large Language Models (LLMs), LLM Evaluation, LLM-as-a-Judge, Prompt Engineering, Structured Information Extraction

**Frameworks & Platforms:** Flutter, Promptfoo, OpenRouter (Claude Sonnet 4.5, GPT-5, GPT-5-mini, GPT-4o), Firebase

**Data & Evaluation:** Ground-Truth Generation, Automated Assertion Testing, Gap Analysis, Document Processing Pipelines
