# 🧠 AI-Powered Narrative Content Engine (PoC)

> **🚧 CURRENT STATUS: Phase 1 - API Resilience & Prompt Design (Active Development)**
> *Currently engineering the backend retry mechanisms and asynchronous data flows.*

## 📌 Project Overview
A full-stack utility tool designed to automate and dynamically generate complex narrative structures (e.g., alternative movie endings, "What If" scenarios). Built to handle the unpredictability of third-party LLMs, this engine focuses on robust API integration, precise prompt engineering, and asynchronous processing.

## 🏗️ System Architecture & Engineering Focus
1. **Client Request:** Next.js frontend sends variables (e.g., Movie Name, Character) to the backend.
2. **Asynchronous Backend:** Spring Boot receives the request and processes it asynchronously to prevent thread-blocking during high-latency AI generation.
3. **Resilient API Integration:** Connects to the **OpenAI API** using custom system prompts to enforce strict JSON output structures. Implements **Retry Mechanisms** and exception handling to gracefully manage rate limits (429) and timeouts.
4. **Delivery:** The structured narrative is returned to the client and rendered dynamically.

## 💻 Tech Stack
* **Backend:** Java, Spring Boot, REST APIs
* **AI Integration:** OpenAI API
* **Frontend:** Next.js, React
* **Concepts:** Async Processing, API Resilience, Fault Tolerance, Prompt Engineering

## ✅ Development Roadmap
- [x] Use-Case Definition & Prompt Structure Design
- [x] Component Data Flow Diagramming
- [ ] Spring Boot Backend & Exception Handling Setup
- [ ] OpenAI API Integration & Retry Logic
- [ ] Next.js Frontend Development
