# 🛡️ AI Security & LLM Red/Blue Teaming Lab

A hands-on security testing and defense lab built to demonstrate vulnerabilities in Large Language Models (LLMs) and AI Agents, along with production-grade mitigation strategies.

This repository covers practical implementations of the **OWASP Top 10 for LLM Applications**, including Direct Prompt Injection, Indirect Prompt Injection in RAG pipelines, and Excessive Agency in Agentic workflows.

---

## 🚀 Key Features & Modules

### 🔹 Week 1: Threat Modeling & Vulnerability Scanning
* Automated security scanning using Python and custom payload execution engines.
* Mapping traditional web application security concepts (SQLi, XSS, Privilege Escalation) to LLM equivalents.

### 🔹 Week 2: Direct Prompt Injection & Delimiter Isolation
* Tested adversarial prompt framing and jailbreak techniques.
* Implemented programmatic **XML Delimiter Isolation** to strictly separate system control logic from untrusted user data.

### 🔹 Week 3: Indirect Prompt Injection & RAG Security
* Simulated document ingestion poisoning attacks (e.g., hidden system overrides in resumes/documents).
* Applied context boundaries and input sanitization to safeguard Retrieval-Augmented Generation (RAG) pipelines.

### 🔹 Week 4: AI Agent Security & Function Safeguards
* Mitigated **Excessive Agency (OWASP LLM08)** during tool/function execution.
* Implemented **Role-Based Access Control (RBAC)** and **Human-in-the-Loop (HITL)** safeguards outside the model layer.

---

## 🛠️ Tech Stack & Prerequisites

* **Language:** Python 3.10+
* **LLM Engine:** [Ollama](https://ollama.com/) running `llama3.2` locally
* **Libraries:** `ollama`, `pydantic`
* **Environment:** VS Code, Windows PowerShell

---

## 📁 Repository Structure

```text
ai-security-lab/
│
├── week1_threat_model.md       # OWASP Top 10 threat mapping analysis
├── week2_defense.py            # XML delimiter defense implementation
├── week2_jailbreak_analysis.md # Direct injection attack breakdown
├── week3_rag_security.py       # Indirect prompt injection test setup
├── week3_rag_analysis.md       # RAG pipeline threat analysis
├── week4_agent_security.py     # RBAC & HITL function guardrails
├── week4_agent_analysis.md     # Agentic security report
├── secure_app.py               # Dual-layer input/output guardrail wrapper
└── README.md                   # Project documentation
