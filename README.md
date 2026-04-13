# MedFolder AI Overview

MedFolder AI is a local-first research prototype for turning medical PDFs into structured, reviewable intelligence.

It is designed for technical evaluation and research workflows, not for diagnosis, treatment, or routine clinical use.

## Screenshot

![MedFolder AI workspace overview](https://github.com/user-attachments/assets/f9c13371-75af-4445-9bfc-79152fa5853c)

## Why it matters

Medical information is often scattered across PDFs from different dates and institutions.  
MedFolder AI explores how these records can be transformed into a more structured, reviewable workspace for research and technical evaluation.

## Core capabilities

- **Medical PDF intake and parsing**  
  Accepts medical PDF documents and prepares them for structured downstream processing.

- **OCR-assisted document recovery**  
  Supports OCR-based handling for noisy, scanned, or imperfect source material.

- **Structured medical extraction**  
  Extracts review-oriented signals such as diagnoses, medications, temporal references, and supporting evidence spans.

- **Hybrid pipeline processing**  
  Combines deterministic logic, heuristic extraction, normalization, confidence scoring, and optional model-assisted stages instead of relying on a single black-box model.

- **Cross-document timeline fusion**  
  Relates findings across multiple documents and dates to support longitudinal review where available.

- **Evidence-linked review surfaces**  
  Organizes extracted findings into inspectable structures rather than presenting opaque final outputs only.

- **Conflict and consistency review**  
  Highlights ambiguity, mismatch, overlap, and case-level review signals across documents and structured findings.

- **Local-first workspace design**  
  Built around privacy-sensitive local processing rather than routine remote handling of raw medical source files.

- **Security-conscious processing model**  
  Explores stronger safeguards beyond local-first handling alone, including controlled data flow, fail-closed contracts, and protected storage and export paths where applicable.

## Architecture overview

MedFolder AI is designed as a local-first document intelligence workspace for technical evaluation and research use.

At a high level, the system consists of several cooperating layers:

1. **Document intake layer**  
   Handles PDF upload, parsing preparation, OCR recovery paths, and source-document preprocessing.

2. **Hybrid extraction pipeline**  
   Converts raw document content into structured intermediate signals using a mix of deterministic parsing, heuristic rules, normalization logic, confidence scoring, and optional ML-assisted stages.

3. **Medical evidence graph**  
   Connects extracted findings to supporting evidence so diagnoses, medications, and related signals remain more reviewable and traceable.

4. **Cross-document fusion and timeline layer**  
   Aligns findings across records and dates to support longitudinal review rather than document-by-document reading only.

5. **Cubes-oriented systems layer**  
   Introduces a modular cube-style execution model for stricter boundaries between processing responsibilities, typed envelopes, and more controlled routing across subsystems.

6. **Meta-optimization and orchestration layer**  
   Explores higher-level orchestration strategies for improving extraction behavior, confidence handling, conflict processing, and workflow routing across the system.

7. **Workspace UI layer**  
   Presents documents, evidence, review state, conflicts, and next-step workflow guidance in an inspectable interface rather than a black-box result screen.

## Systems and infrastructure ideas

MedFolder AI is not built around a single end-to-end model.  
Its direction is closer to a hybrid medical document intelligence stack with several interacting components and architectural safeguards.

This includes work on ideas such as:

- **hybrid extraction pipelines**
- **medical evidence graphs**
- **cross-document reasoning**
- **timeline fusion**
- **conflict and consistency detection**
- **meta-optimizer concepts for case-level orchestration**
- **cube-style execution boundaries**
- **Arrow-oriented handling for larger tabular data paths**
- **architect-layer style evaluation and workflow control**
- **local-first review surfaces for human inspection**

## Privacy and security direction

MedFolder AI is designed around a **local-first and privacy-sensitive workflow**.

The project direction also includes stronger technical safeguards beyond the local-only default where applicable, such as:

- **restricted data movement**
- **controlled execution boundaries**
- **fail-closed contract thinking**
- **safer storage and export paths**
- **encryption-oriented handling for sensitive artifacts**
- **structured separation between processing layers**

Where needed, protected local storage and artifact handling may include encryption-oriented mechanisms such as **AES-based protection** for sensitive data paths or retained outputs.

## Design principles

- **Local-first by default**
- **Privacy-sensitive by design**
- **Human review before trust**
- **Explainability over black-box presentation**
- **Structured evidence over raw document chaos**
- **Hybrid pipeline thinking over single-model dependence**
- **Security-aware architecture, not just UI-level privacy language**
- **Research prototype, not clinical automation**

## Current scope

MedFolder AI is currently a **research prototype**.  
It is intended for demonstration, technical evaluation, and exploratory research workflows.

The public repository provides a project overview only.  
The main implementation remains private at this stage.

## Important notice

MedFolder AI is not a medical device.  
It is not intended for diagnosis, treatment, clinical decision-making, emergency use, or routine patient care.

Outputs may be incomplete, inaccurate, or misleading and always require qualified human review.

## Planned public additions

- additional screenshots
- feature walkthrough
- development roadmap
