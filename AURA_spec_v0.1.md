# AURA Protocol — Attribution & Usage Reporting for AI

**Version 0.1 | July 2025**  
**License: CC-BY-SA 4.0**  
**Maintainer: Fausto D. Cortés Rojas**

---

## 🌍 Foundational Manifesto

Generative AI can now produce textual, visual, and functional content at scale, with increasing quality and realism. This new paradigm demands robust answers to questions of **authorship**, **integrity**, and **traceability**. The ease of generation must not erase the duty of disclosure.

**AURA** (Attribution & Usage Reporting for AI) proposes a formal, open, and verifiable structure to document and communicate the involvement of AI in the creative process. It is not about limiting usage, but enabling **transparent and reproducible attribution**.

---

## 🎯 Objectives

- Provide a structured and machine-readable format to attribute AI-generated content.
- Support version control, reproduction, and provenance auditing.
- Encourage ethical and transparent authorship practices.
- Enable downstream consumers (journals, institutions, users) to evaluate AI involvement with clarity.

---

## ⚖️ Guiding Principles

| Principle       | Description |
|----------------|-------------|
| Neutrality      | Does not judge the use of AI — it documents it. |
| Interoperability| Compatible with various media types and workflows. |
| Verifiability   | Uses content hashes and session metadata. |
| Modularity      | Extensible to text, code, image, audio, or video. |
| Consent         | Voluntary participation, cryptographically traceable. |

---

## 📦 AURA Metadata Block (Extended Schema)

AURA metadata blocks are written in JSON or YAML and can be embedded or attached to content.

### ✅ Example (JSON format)

```json
{
  "aura_version": "0.1",
  "uid": "AURA-2025-000001",
  "timestamp": "2025-07-11T23:10Z",
  "model": "ChatGPT 4.0",
  "provider": "OpenAI",
  "endpoint": "https://chat.openai.com/",
  "session_id": "f09ae12d-4837-4eab-b50b-ef6d7ef4b9f3",
  "prompt": "Describe the impact of AI on education",
  "full_completion": "AI can positively impact education by...",
  "temperature": 0.7,
  "max_tokens": 800,
  "user_edit": false,
  "editor_identity": null,
  "content_hash": "a0f4c9bd7e24af91fabc123c78a94dc82f7f8ab31c2f3c0f098a3a2b1c0e5db2e",
  "file_origin": "article-draft.md",
  "license": "CC-BY-4.0",
  "usage_context": "Academic article (Introduction section)",
  "notes": "Generated content with no manual revision."
}
