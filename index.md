## Selected Projects in AI Engineering, Data Science & Machine Learning

Building end-to-end AI systems and data products combining LLMs, machine learning, analytics, ETL pipelines, and interactive web applications.

---

# 🏦 CRM AI — Banking Assistant

Conversational banking assistant combining **Tool Calling** and **RAG** built on the Anthropic Claude API. Agentic system where Claude autonomously decides which tools to use based on user intent.

### Features

* Agentic tool calling — Claude decides which tool to invoke based on intent
* 6 custom tools (balance, payments, limit requests, semantic search)
* Hybrid RAG: semantic chunking over a 48-page policy document
* ChromaDB + VoyageAI embeddings (`voyage-3-large`)
* Flask frontend with real-time SSE streaming
* Dockerized with automatic DB setup and RAG indexing on first run

### Tech Stack

Python · Anthropic Claude API · ChromaDB · VoyageAI · Flask · SQLite · Docker

<div class="project-actions">
  <a class="project-button secondary" href="https://github.com/facurabinovich/crm-ai" target="_blank">GitHub Repo</a>
</div>

**Tool Calling** — Claude consulta saldo, fechas y límite de tarjeta en tiempo real:

<div class="project-gallery">
  <img src="https://raw.githubusercontent.com/facurabinovich/crm-ai/main/gifs/tool-calling%20example.gif"/>
</div>

**RAG** — búsqueda semántica sobre la base de conocimiento del banco:

<div class="project-gallery">
  <img src="https://raw.githubusercontent.com/facurabinovich/crm-ai/main/gifs/rag%20example.gif"/>
</div>

---

# 🎵 Tailorlist

Full-stack music analytics and playlist intelligence platform powered by Spotify data.

### Features

* Spotify API integration
* Automated ETL pipelines
* MySQL star schema
* Audio feature analysis
* Playlist comparison
* Duplicate detection
* Clustering and classification models
* Interactive multi-page web application

### Tech Stack

Python · MySQL · Streamlit · scikit-learn · Plotly · Spotify API

<div class="project-actions">
  <a class="project-button" href="https://www.tailorlist.app/" target="_blank">Live Demo</a>
  <a class="project-button secondary" href="https://github.com/facurabinovich/tailorlist" target="_blank">GitHub Repo</a>
</div>

<div class="project-gallery">
  <img src="images/tailorlist_1.png?raw=true"/>
  <img src="images/tailorlist_2.png?raw=true"/>
  <img src="images/tailorlist_3.png?raw=true"/>
  <img src="images/tailorlist_4.png?raw=true"/>
</div>

---

# 🎾 ATP Tennis Match Predictor

End-to-end ML system trained on 66k+ ATP matches (2000–2024).

### Highlights

* LightGBM predictive model
* 85 engineered tennis-specific features
* Validation AUC: **0.7599**
* 2025 Test Accuracy: **67.59%**
* Streamlit deployment
* MySQL backend

### Tech Stack

Python · LightGBM · scikit-learn · pandas · MySQL · Streamlit

<div class="project-actions">
  <a class="project-button" href="https://facustennispredictor.streamlit.app/" target="_blank">Live Demo</a>
  <a class="project-button secondary" href="https://github.com/facurabinovich/tennis-match-predictor" target="_blank">GitHub Repo</a>
</div>

<div class="project-gallery">
  <img src="images/tennis_1.png?raw=true"/>
  <img src="images/tennis_2.png?raw=true"/>
  <img src="images/tennis_3.png?raw=true"/>
</div>

---

## About Me

Systems Engineer focused on AI Engineering and Data Science, building end-to-end systems that combine LLMs, machine learning, and data pipelines.

Currently working as a Data Analyst developing ETL pipelines, dashboards, and analytics solutions using Python, SQL, and cloud technologies.

Interested in:

* AI Engineering & LLM Applications
* Machine Learning & Predictive Modeling
* Recommendation Systems
* End-to-End Data Products

---

## Tech Stack

### Languages & Databases

* Python
* SQL (MySQL and SQLite)
* Bash

### AI Engineering

* Anthropic Claude API
* Tool Calling & Agentic Systems
* RAG (Retrieval-Augmented Generation)
* ChromaDB · VoyageAI
* Docker

### Data Science & ML

* pandas
* NumPy
* scikit-learn
* LightGBM
* XGBoost
* TensorFlow
* PyTorch

### Data Engineering & Visualization

* ETL Pipelines
* REST APIs
* Streamlit
* Plotly
* Power BI
* Knowage

### Cloud & Deployment

* AWS
* Railway
* Neon
* Streamlit Cloud

---

## Connect

* LinkedIn: https://www.linkedin.com/in/facundo-rabinovich
* GitHub: https://github.com/facurabinovich

---

<p style="font-size:11px; color: #8b949e;">
Template originally forked from
<a href="https://github.com/evanca/quick-portfolio" style="color: #58a6ff;">evanca</a>
</p>
