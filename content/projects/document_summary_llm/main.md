---
title: "DocChat: Intelligent Document Retrieval & Verification for Technical Data"
summary: "Self-correcting multi-agent RAG for audits. Built with LangGraph, Docling & Modal."
date: 2026-01-18
authors:
    - admin
type: project
content_meta:
  content_type: 'App'
links:
  - type: code
    name: GitHub Repo
    url: https://github.com/EstevanFisk/document_summary_llm.git
    icon: brands/github
  - type: code
    name: "Launch Live Demo"
    url: "/projects/document_summary_llm/demo"
tags:
  - Python
  - LLM
  - Agentic AI
  - AI
  - Multi-modal
  - Generative AI
  - Gradio
  - Modal
  - Gemini
  - OpenAI
  - Docling
sitemap: true
share: false
featured: true
build:
  list: always
  render: always
image:
  filename: docchat_featured.png
  #weight: 1
draft: false
---

> **A high-precision RAG system designed to bridge the "Hallucination Gap" in technical document audit.**

---

<div style="display: flex; justify-content: center; flex-wrap: nowrap; gap: 4px; margin-bottom: 0px; margin-top: -50px; transform: scale(1.00); transform-origin: center;">
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python&logoColor=white" alt="Python 3.10+"></a>
  <a href="https://ai.google.dev/"><img src="https://img.shields.io/badge/LLM-Gemini_1.5-blueviolet?style=flat&logo=googlegemini&logoColor=white" alt="Gemini 1.5 LLM"></a>
  <a href="https://openai.com/"><img src="https://img.shields.io/badge/LLM-OpenAI-412991?style=flat&logo=openai&logoColor=white" alt="OpenAI Backup LLM"></a>
  <a href="https://langchain-ai.github.io/langgraph/"><img src="https://img.shields.io/badge/Agents-LangGraph-orange?style=flat" alt="LangGraph Agents"></a>
  <a href="https://modal.com"><img src="https://img.shields.io/badge/Compute-Modal-green?style=flat&logo=modal" alt="Modal Compute"></a>
</div>

<div style="display: flex; justify-content: center; flex-wrap: nowrap; gap: 4px; margin-bottom: 0px; margin-top: -50px; transform: scale(1.00); transform-origin: center;">
  <a href="https://www.trychroma.com/"><img src="https://img.shields.io/badge/Vector-Chroma-yellow?style=flat&logo=googlecloud&logoColor=white" alt="Chroma Vector DB"></a>
  <a href="https://github.com/DS4SD/docling"><img src="https://img.shields.io/badge/Parsing-Docling-blue?style=flat" alt="Docling Parsing"></a>
  <a href="https://ai.google.dev/models/embeddings"><img src="https://img.shields.io/badge/Embeds-Text--004-9C27B0?style=flat&logo=google" alt="Gemini Embeddings"></a>
</div>

<div style="display: flex; justify-content: center; flex-wrap: nowrap; gap: 4px; margin-bottom: -30px; margin-top: -50px; transform: scale(1.00); transform-origin: center;">
  <a href="https://en.wikipedia.org/wiki/Data_science"><img src="https://img.shields.io/badge/Data_Scientist-0077B5?style=flat&logo=googlesheets&logoColor=white" alt="Data Scientist"></a>
  <a href="https://en.wikipedia.org/wiki/Statistics"><img src="https://img.shields.io/badge/M.S._Stats-C41E3A?style=flat&logo=icloud&logoColor=white" alt="M.S. Statistics"></a>
  <a href="https://en.wikipedia.org/wiki/Stoicism"><img src="https://img.shields.io/badge/Stoic-aa9a73?style=flat&logo=probot&logoColor=white" alt="Stoicism"></a>
</div>

---


## 🎖️ The Inspiration: From Defense Analysis to Data Science
During my time as a **Cost Analyst for the U.S. Air Force**, I navigated the "Document Maze"—thousands of hours spent auditing dense technical proposals, program descriptions, and complex contract policy manuals. In high-stakes defense environments, missing a single footnote in a 500-page document isn't just an inconvenience; it can lead to multi-million dollar discrepancies.

I built **DocChat** because I knew there was a better way to ensure 100% accuracy without the human burnout. This tool moves beyond simple "Chat-with-PDF" wrappers to create a system that **thinks like an analyst**: verifying its own claims and handling complex layouts that traditional AI often fails to parse.

---

## 🚀 The Industry Problem: Why I Built This
Generic AI often fails in specialized sectors like Defense, Finance, or Law because it lacks **rigor**. I built **DocChat** because I knew there was a better way to ensure 100% accuracy without the human burnout. I moved beyond a simple "Chat-with-PDF" wrapper to create a system that **thinks like an analyst**:

* **Trust, but Verify:** Just as an analyst cross-references sources, DocChats’ **Verification Agent** checks every AI claim against the original source text.
* **Context is King:** Using **Docling**, I ensured the AI understands table structures and complex layouts—elements where standard RAG systems usually break.
* **The "Full-Stack" Advantage:** By deploying this on **Modal** with a **Dual-LLM (Gemini/OpenAI) failover**, I’ve demonstrated the ability to take a high-level business need and turn it into a resilient, scalable, and cost-effective cloud application.

---


## 🏗️ Architecture & Engineering
This project is a full-stack engineering demonstration of how to build and deploy a heavy RAG pipeline on serverless infrastructure.

### **The Multi-Agent Orchestration**
Instead of a linear prompt, the app utilizes a **LangGraph-driven state machine** that mimics a human research workflow:
1. **The Research Agent:** Conducts a **Hybrid Search** (BM25 + Vector) to find relevant data.
2. **The Verification Agent:** Cross-checks every generated claim against the original source text to eliminate hallucinations.
3. **The Self-Correction Loop:** Automatically triggers a re-run of the research phase if unsupported statements are detected.

```mermaid
graph TD
    Start([<b>START</b>]) --> Relevance[<b>Relevance Checker</b>]
    
    Relevance -- "Relevant" --> Research[<b>Research Agent</b>]
    Relevance -- "Irrelevant" --> End([<b>END</b>])
    
    Research --> Verify[<b>Verification Agent</b>]
    
    Verify -- "Needs Correction" --> Research
    Verify -- "Verified" --> End

    style Start fill:#f9f,stroke:#333,stroke-width:2px
    style End fill:#bbf,stroke:#333,stroke-width:2px
    style Relevance fill:#e1f5fe,stroke:#01579b
    style Research fill:#e8f5e9,stroke:#2e7d32
    style Verify fill:#fff3e0,stroke:#ef6c00
```



### **Technical Infrastructure**
* **Serverless Intelligence:** Deployed on **Modal**, utilizing Infrastructure-as-Code (IaC) to manage GPU resources and custom container environments.
* **Layout-Aware Parsing:** Implemented **IBM Docling** to treat PDFs as visual structures, ensuring the AI understands multi-column tables and headers that standard parsers merge into "text soup."
* **Reliability Engineering:** Developed a **Dual-LLM Failover** strategy using **Gemini 2.5 Flash** as the primary engine and **GPT-4o-mini** as an automatic fallback.

---

## 🛠️ Tech Stack
* **Orchestration:** LangGraph
* **LLMs:** Gemini 2.5 Flash, OpenAI GPT-4o-mini
* **Data Engineering:** IBM Docling, RapidOCR, ChromaDB
* **Infrastructure:** Modal (Serverless Cloud), Python 3.12, Gradio (UI)



{{< cards >}}
  {{< card url="/projects/document_summary_llm/demo" title="DocChat App" icon="adjustments-vertical" subtitle="Experience DocChat live!">}}
{{< /cards >}}