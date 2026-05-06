# Medfolder AI — Progress Update (May 2026)

Clinical AI infrastructure prototype focused on local-first medical document intelligence, evidence-grounded reasoning, and explainable clinical workflows.

---

# Current State

Medfolder AI has now reached a stage where the complete prototype workflow is visible end-to-end:

Medical PDF upload → structured extraction → clinical fusion → conflict handling → evidence-linked PDF review → deterministic brief drafting → optional local Ollama smoothing.

The current focus has shifted from pure feature implementation toward:
- robustness
- explainability
- workflow consistency
- demo hardening
- architectural stabilization

The project is being developed as a deterministic-first clinical document intelligence system rather than a generic medical chatbot or simple LLM wrapper.

---

# Current Prototype Workflow

## 1. Medical Document Upload
- Multi-document PDF upload
- Local-first processing pipeline
- OCR fallback support
- Structured document ingestion
- Workspace-oriented review flow

---

## 2. Structured Extraction Layer

The extraction pipeline currently processes:
- diagnoses
- medications
- procedures
- laboratory references
- document metadata
- temporal information
- section structures

The system combines:
- deterministic heuristics
- section-aware extraction
- rule-based clinical logic
- conservative ML-assisted ranking signals

A major focus is maintaining clinical traceability and minimizing hallucinated structure generation.

---

## 3. Clinical Fusion Layer

The fusion layer merges information across multiple medical documents into:
- longitudinal case structures
- primary diagnosis candidates
- secondary diagnoses
- medication overviews
- timeline-oriented summaries
- reviewable clinical states

The current architecture prioritizes:
- current vs historical findings
- acute vs chronic relevance
- explicit uncertainty handling
- deterministic ranking transparency

---

## 4. Conflict Detection & Clinical Review

Instead of hiding inconsistencies, Medfolder explicitly surfaces:
- competing primary diagnoses
- conflicting document states
- uncertain extractions
- low-confidence OCR situations
- review-required clinical ambiguities

The system is designed around a human-in-the-loop review philosophy.

Clinical review remains central to the workflow.

---

## 5. Evidence-Linked PDF Navigation

Structured outputs remain connected to:
- original PDF pages
- highlighted source regions
- evidence anchors
- document sections
- source references

The goal is direct verifiability of extracted clinical information inside the original medical document.

Current development includes:
- coordinate-based highlighting
- OCR-aware evidence handling
- multi-page highlight propagation
- Safari-specific rendering stabilization

---

## 6. Clinical Workspace

The workspace architecture is evolving toward a clinical working environment rather than a traditional dashboard.

Current components include:
- structured diagnosis panels
- medication review
- timeline-oriented navigation
- PDF evidence reader
- document track navigation
- conflict-aware review flows
- deterministic summary generation

The reader and structured outputs remain tightly coupled.

---

## 7. Deterministic Brief Generation

The system can generate deterministic clinical brief drafts based on structured pipeline outputs.

Example sections:
- Anlass
- Leitdiagnose
- Nebendiagnosen
- Verlauf
- Therapie
- Empfehlungen

The deterministic layer is intended to preserve:
- auditability
- explainability
- source traceability
- stable clinical structure

---

## 8. Optional Local Ollama Integration

Optional local LLM integration via Ollama is used for:
- wording refinement
- readability improvements
- language smoothing

Important architectural principle:

The LLM layer does not define structured clinical facts.

Structured outputs are generated first through deterministic processing and only optionally reformulated afterward.

This separation is intentional and central to the current architecture.

---

# Core Architectural Principles

## Local-first Processing

Medical documents should not require mandatory cloud processing.

The current prototype is designed around local workflows and privacy-sensitive handling.

---

## Deterministic-first Reasoning

Core clinical structure should not depend entirely on probabilistic LLM behavior.

Deterministic extraction and reviewability remain primary architectural goals.

---

## Evidence Grounding

Structured outputs should remain traceable to the original PDF source whenever possible.

---

## Explainability

Conflicts, uncertainty, confidence issues, and competing interpretations should remain visible.

---

## Human-in-the-loop

The system is intended to support structured clinical review — not replace clinical decision-making.

---

# Current Technical Focus

Current engineering priorities include:
- extraction robustness
- PDF evidence stability
- conflict calibration
- longitudinal reasoning
- OCR reliability
- workflow consistency
- UI stabilization
- monolith reduction
- auditability infrastructure
- deterministic explainability tooling

---

# Current Architectural Areas

Current prototype areas include:
- hybrid deterministic extraction pipeline
- clinical fusion layer
- evidence-linked PDF viewer
- Architect Layer for scoring/debugging
- workspace review system
- deterministic brief drafting
- local Ollama integration
- clinical confidence signaling
- conflict-aware diagnosis handling

---

# Technology Stack

Current technologies include:
- Next.js
- React
- TypeScript
- PDF.js
- local-first workflow architecture
- Ollama local inference
- deterministic extraction systems
- hybrid scoring pipeline

---

# Current Challenges

Several areas are still under active development and refinement:

- OCR variability between documents
- PDF highlighting edge cases
- multi-document temporal reasoning
- extraction reliability in noisy layouts
- calibration of diagnosis conflicts
- UI consistency
- architectural modularization
- deterministic/ML interaction boundaries

The project is currently in an active hardening and stabilization phase.

---

# Current Direction

The current direction is moving toward:
- explainable clinical document intelligence
- evidence-grounded workflows
- review-oriented medical AI systems
- privacy-sensitive local processing
- deterministic clinical infrastructure
- longitudinal document understanding

---

# Prototype Status & Limitations

Medfolder AI is currently an experimental research prototype.

Important limitations:
- extraction errors may occur
- OCR quality may vary significantly
- conflict handling is still evolving
- UI inconsistencies are present
- longitudinal reasoning remains incomplete
- no clinical validation has been performed
- no regulatory approval exists
- outputs may be incomplete or incorrect

The system must not be used for real clinical diagnosis, treatment decisions, or autonomous medical decision-making.

---

# Screenshots & Demonstration

Current demonstrations show:
- multi-document clinical workflows
- evidence-linked PDF navigation
- structured extraction
- conflict-aware review flows
- deterministic brief drafting
- local Ollama-assisted wording

The attached screenshots/videos use dummy/mock data.

---

# Disclaimer

This repository represents an active research and prototype development project.

The system is incomplete and under continuous architectural and clinical evaluation.

Outputs may contain:
- extraction mistakes
- missing information
- inconsistent reasoning
- incomplete conflict handling
- unstable UI behavior

The project is intended for:
- technical evaluation
- workflow exploration
- prototype research
- explainability experimentation

It is not intended for production clinical use.
