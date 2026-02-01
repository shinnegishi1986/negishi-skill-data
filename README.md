# negishi-skill-data

Dataset for studying skills and generating derivative content (slides, videos, PRDs, and more) using AI tools such as NotebookLM and other LLM-based services. 

***

## Overview

- **Name**: negishi-skill-data  
- **Purpose**: Centralized corpus about skills, roles, and workflows for use as a private knowledge base in AI tools. Typical outputs include:
  - Study notes and Q&A
  - Slide decks and training materials
  - Explainer videos and scripts
  - Product requirement documents (PRDs) and planning docs 
- **Intended tools**: NotebookLM, GPT-style chat systems, RAG pipelines, vector-search backends. 
- **Current version**: 0.1.0  
- **Language**: Primarily Japanese and English (mixed is allowed; adjust as needed).  

***

## Contents

Adjust this section to match your actual files.

- `docs/`
  - Source documents (Markdown, PDF, text, slides exports) describing skills, processes, and domain knowledge.
- `tables/`
  - Structured data (CSV, TSV, JSON) such as skill matrices, role definitions, checklists.
- `examples/`
  - Example PRDs, slide outlines, video scripts, FAQs.
- `meta/`
  - Tag lists, ontologies, and mappings (e.g., skill → role, skill → level).
- `README.md`
  - This description file.

For each file or folder, you are encouraged to add a short description (what it contains, language, update date) directly in this section. 

***

## Typical Use Cases

- Create learning plans or **study** materials from the dataset (summaries, quizzes, concept maps). 
- Auto-generate slide outlines or full slide notes for internal training.  
- Draft PRDs from skill or process descriptions (e.g., “Create a PRD for a training portal based on these skills”). 
- Generate video scripts, narration text, and storyboards for explainer content.  
- Answer Q&A about skills, roles, responsibilities, workflows, or best practices.

***

## How to Use with NotebookLM

1. Prepare documents
   - Use stable formats (PDF, TXT, MD, DOCX, CSV) and ensure each file has a clear title and, if possible, a short preface section explaining its context. 
2. Upload as sources
   - In NotebookLM, create a new notebook and upload the files from `docs/`, `tables/`, and `examples/` as “source documents.”
3. Configure prompts
   - Example prompts:
     - “Summarize all beginner-level skills for role X and output as bullet points.”
     - “Generate a 10-slide outline to teach topic Y to junior engineers.”
     - “Draft a PRD for feature Z using only the uploaded skill definitions.”
4. Iterate and refine
   - Add more documents or updated skill definitions as needed and keep this README in sync with structural changes. 

***

## Data Structure and Conventions

You can adapt these suggestions to your actual schema.

- **Skill IDs**: Stable identifiers like `SKILL_FRONTEND_BASIC`, used across tables and documents.  
- **Skill levels**: e.g., `beginner`, `intermediate`, `advanced`, `expert`.  
- **Role mappings**: Each role links to multiple skills with priority or importance scores (e.g., 1–5).  
- **File naming**:
  - `skill_[domain]_[level].md` (e.g., `skill_backend_intermediate.md`)
  - `role_[name].md` (e.g., `role_product_manager.md`)
  - `example_[artifact]_[topic].md` (e.g., `example_prd_lms_platform.md`)

These conventions improve reuse and interpretability for people and AI systems. 

***

## Methodology

Document here how you created and maintain the dataset (edit this section as needed).

- **Source**: Internal documentation, training materials, personal notes, and curated public references.  
- **Curation**: Consolidated overlapping documents, normalized terminology, added IDs, and standardized levels and tags.  
- **Update policy**: Increment minor version when adding or revising content; increment major version if structure or schema changes significantly. 

***

## Privacy, Licensing, and Usage

- **Personal data**: Ensure the dataset does not include real personal data, secrets, or confidential business information, or clearly mark and exclude such files from AI uploads. 
- **Copyright**: Include only text and data you own or are allowed to reuse; for third-party content, summarize instead of copying verbatim when in doubt. 
- **License**: Specify your chosen license (e.g., CC BY 4.0, CC BY-NC-SA 4.0, or “Internal use only”) here and in a separate `LICENSE` file if applicable. 

Example:

> License: CC BY-NC-SA 4.0 – You may share and adapt with attribution, non-commercial use, and share-alike terms.

***

## Recommended Prompts

You can store or extend these as `meta/prompts.md`.

- “From these skill definitions, create a one-page study guide for a beginner.”  
- “Generate a detailed PRD outline for a product that teaches these skills to university students.” 
- “Create a script for a 5‑minute video introducing these skills to new hires.”  
- “Compare the skill requirements of role A and role B and output as a Markdown table.”  

***

## Changelog

- **0.1.0** – Initial structure and draft documentation for `negishi-skill-data`.