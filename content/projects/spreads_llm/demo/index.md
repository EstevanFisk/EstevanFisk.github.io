---
title: "LLM Spreads: Demo"
date: 2026-02-14
authors:
    - admin
build:
  list: never
  render: always
#weight: 1
draft: false
---

---

<div style="display: flex; justify-content: center; flex-wrap: nowrap; gap: 4px; margin-bottom: 0px; margin-top: -50px; transform: scale(1.00); transform-origin: center;">
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3.10+-blue?style=flat&logo=python&logoColor=white" alt="Python 3.10+"></a>
  <a href="https://ai.google.dev/"><img src="https://img.shields.io/badge/LLM-Gemini_2.0-blueviolet?style=flat&logo=googlegemini&logoColor=white" alt="Gemini 1.5 LLM"></a>
  <a href="https://openai.com/"><img src="https://img.shields.io/badge/LLM-OpenAI-412991?style=flat&logo=openai&logoColor=white" alt="OpenAI Backup LLM"></a>
  <a href="https://langchain-ai.github.io/langgraph/"><img src="https://img.shields.io/badge/Agents-LangGraph-orange?style=flat" alt="LangGraph Agents"></a>
  <a href="https://modal.com"><img src="https://img.shields.io/badge/Compute-Modal-green?style=flat&logo=modal" alt="Modal Compute"></a>
</div>

<div style="display: flex; justify-content: center; flex-wrap: nowrap; gap: 4px; margin-bottom: 0px; margin-top: -50px; transform: scale(1.00); transform-origin: center;">
  <a href="https://github.com/DS4SD/docling"><img src="https://img.shields.io/badge/Parsing-Docling-blue?style=flat" alt="Docling Parsing"></a>
  <a href="https://ai.google.dev/models/embeddings"><img src="https://img.shields.io/badge/Embeds-Text--004-9C27B0?style=flat&logo=google" alt="Gemini Embeddings"></a>
  <a href="https://streamlit.io/"><img src="https://img.shields.io/badge/Frontend-Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white" alt="Streamlit"></a>
</div>

<div style="display: flex; justify-content: center; flex-wrap: nowrap; gap: 4px; margin-bottom: -30px; margin-top: -50px; transform: scale(1.00); transform-origin: center;">
  <a href="https://en.wikipedia.org/wiki/Data_science"><img src="https://img.shields.io/badge/Data_Scientist-0077B5?style=flat&logo=googlesheets&logoColor=white" alt="Data Scientist"></a>
  <a href="https://en.wikipedia.org/wiki/Statistics"><img src="https://img.shields.io/badge/M.S._Stats-C41E3A?style=flat&logo=icloud&logoColor=white" alt="M.S. Statistics"></a>
  <a href="https://en.wikipedia.org/wiki/Stoicism"><img src="https://img.shields.io/badge/Stoic-aa9a73?style=flat&logo=probot&logoColor=white" alt="Stoicism"></a>
</div>

---

## ⚖️ Deployment & Performance
This application is deployed using a **Serverless Architecture (Modal)**.

- **Cost Efficiency:** To minimize overhead, the infrastructure remains at zero when not in use. You are only billed for the exact seconds the code is running.

- **The "Cold Start" Trade-off:** Upon the first request, the environment takes ~30-60 seconds to spin up the container and load the LLM/Vector index into memory. Subsequent requests are sub-second.

- **Why this approach?** For a portfolio project, this demonstrates the ability to deploy production-grade AI without the high monthly cost of an "always-on" GPU server.

*(Note: The app runs on a cold-start architecture to save costs. Please allow ~30-60 seconds for the first request as the container spins up. Run time for example pdf `Fastenal Report` takes ~45-60 seconds as Docling can take a while to parse the file.)*

---

<p style="text-align: center; font-size: 0.9em; margin-top: 10px;">
  <a href="https://estevan-fisk--llm-spreads-app-run.modal.run" target="_blank" rel="noopener noreferrer">
    Open App Externally in New Tab ↗
  </a>
</p>


<div style="border: 1px solid #e5e7eb; border-radius: 8px; overflow: hidden;">
  <iframe
    src="https://estevan-fisk--llm-spreads-app-run.modal.run"
    width="100%"
    height="1200px"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen
  ></iframe>
</div>


