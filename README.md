# 🕸️ EchoSwarm Engine v1.0

EchoSwarm is a high-performance, asynchronous multi-agent simulation framework designed to model complex social dynamics and behavioral patterns using Large Language Models (LLMs).

Unlike standard synchronous wrappers, EchoSwarm utilizes a **decoupled microservices architecture** to handle large-scale agent interactions without blocking the main execution thread.

---

## 🚀 Key Architectural Features

* **Asynchronous Core:** Built with FastAPI and `asyncio` to manage parallel LLM inference tasks.
* **Parametric Agent Design:** Agents are instantiated via psychometric vectors (Aggressiveness, Rationality, Bias, Ideology) rather than static prompts.
* **State Persistence:** Automatic telemetry export to structured JSON for post-simulation data analysis and visualization.
* **Scalable Pipeline:** Designed to be integrated with message brokers like RabbitMQ or Kafka for million-agent simulations.

---

## 🏗️ Project Structure

* `main.py`: The high-performance REST API and background worker engine.
* `app.py`: A Streamlit-based control room for real-time simulation management.
* `requirements.txt`: Environment dependencies.

---

## 🚦 Quick Start

### 1. Install Dependencies
`pip install fastapi uvicorn httpx pydantic streamlit pandas`

### 2. Launch the Engine (Backend)
`uvicorn main:app --reload`

### 3. Launch the Dashboard (Frontend)
`streamlit run app.py`

---

## Research Goals

1. **Information Warfare:** Studying echo chamber formation.
2. **Social Triggers:** Testing the impact of news on demographic clusters.
3. **Scalability:** Analyzing concurrency limits of LLM-based agents.

---
*Developed for research purposes in Swarm Intelligence and Behavioral Modeling.*
Developed for research purposes in Swarm Intelligence and Behavioral Modeling.
