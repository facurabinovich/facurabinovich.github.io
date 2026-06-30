<div class="project-nav">
  <a href="#crm-ai">🏦 CRM AI</a>
  <a href="#tailorlist">🎵 Tailorlist</a>
  <a href="#tennis">🎾 Tennis Predictor</a>
  <a href="#about">About Me</a>
</div>

## Selected Projects in AI Engineering, Data Science & Machine Learning

Building end-to-end AI systems and data products combining LLMs, machine learning, analytics, ETL pipelines, and interactive web applications.

<div class="project-card" id="crm-ai" markdown="1">

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

<div class="tech-stack">
  <span class="tech-badge">Python</span>
  <span class="tech-badge">Anthropic Claude API</span>
  <span class="tech-badge">ChromaDB</span>
  <span class="tech-badge">VoyageAI</span>
  <span class="tech-badge">Flask</span>
  <span class="tech-badge">SQLite</span>
  <span class="tech-badge">Docker</span>
</div>

<div class="project-actions">
  <a class="project-button secondary" href="https://github.com/facurabinovich/crm-ai" target="_blank">⬡ GitHub Repo</a>
</div>

**Tool Calling** — Claude consulta saldo, fechas y límite de tarjeta en tiempo real:

<div class="project-gallery">
  <img src="https://raw.githubusercontent.com/facurabinovich/crm-ai/main/gifs/tool-calling%20example.gif"/>
</div>

**RAG** — búsqueda semántica sobre la base de conocimiento del banco:

<div class="project-gallery">
  <img src="https://raw.githubusercontent.com/facurabinovich/crm-ai/main/gifs/rag%20example.gif"/>
</div>

</div>

<div class="project-card" id="tailorlist" markdown="1">

# 🎵 Tailorlist

Full-stack music analytics and playlist intelligence platform powered by Spotify data.

### Features

* Spotify API integration
* Automated ETL pipelines
* MySQL star schema
* Audio feature analysis
* Playlist comparison & duplicate detection
* Clustering and classification models
* Interactive multi-page web application

### Tech Stack

<div class="tech-stack">
  <span class="tech-badge">Python</span>
  <span class="tech-badge">MySQL</span>
  <span class="tech-badge">Streamlit</span>
  <span class="tech-badge">scikit-learn</span>
  <span class="tech-badge">Plotly</span>
  <span class="tech-badge">Spotify API</span>
</div>

<div class="project-actions">
  <a class="project-button" href="https://www.tailorlist.app/" target="_blank">↗ Live Demo</a>
  <a class="project-button secondary" href="https://github.com/facurabinovich/tailorlist" target="_blank">⬡ GitHub Repo</a>
</div>

<div class="project-gallery">
  <img src="images/tailorlist_1.png?raw=true"/>
  <img src="images/tailorlist_2.png?raw=true"/>
  <img src="images/tailorlist_3.png?raw=true"/>
  <img src="images/tailorlist_4.png?raw=true"/>
</div>

</div>

<div class="project-card" id="tennis" markdown="1">

# 🎾 ATP Tennis Match Predictor

End-to-end ML system trained on 66k+ ATP matches (2000–2024).

### Highlights

* LightGBM predictive model
* 85 engineered tennis-specific features
* Validation AUC: **0.7599**
* 2025 Test Accuracy: **67.59%**
* Streamlit deployment with MySQL backend

### Tech Stack

<div class="tech-stack">
  <span class="tech-badge">Python</span>
  <span class="tech-badge">LightGBM</span>
  <span class="tech-badge">scikit-learn</span>
  <span class="tech-badge">pandas</span>
  <span class="tech-badge">MySQL</span>
  <span class="tech-badge">Streamlit</span>
</div>

<div class="project-actions">
  <a class="project-button" href="https://facustennispredictor.streamlit.app/" target="_blank">↗ Live Demo</a>
  <a class="project-button secondary" href="https://github.com/facurabinovich/tennis-match-predictor" target="_blank">⬡ GitHub Repo</a>
</div>

<div class="project-gallery">
  <img src="images/tennis_1.png?raw=true"/>
  <img src="images/tennis_2.png?raw=true"/>
  <img src="images/tennis_3.png?raw=true"/>
</div>

</div>

---

<div id="about" markdown="1">

## About Me

Systems Engineer focused on AI Engineering and Data Science, building end-to-end systems that combine LLMs, machine learning, and data pipelines.

Currently working as a Data Analyst developing ETL pipelines, dashboards, and analytics solutions using Python, SQL, and cloud technologies.

Interested in:

* AI Engineering & LLM Applications
* Machine Learning & Predictive Modeling
* Recommendation Systems
* End-to-End Data Products

## Tech Stack

### Languages & Databases

<div class="tech-stack">
  <span class="tech-badge">Python</span>
  <span class="tech-badge">SQL · MySQL</span>
  <span class="tech-badge">SQLite</span>
  <span class="tech-badge">Bash</span>
</div>

### AI Engineering

<div class="tech-stack">
  <span class="tech-badge">Anthropic Claude API</span>
  <span class="tech-badge">Tool Calling</span>
  <span class="tech-badge">RAG</span>
  <span class="tech-badge">ChromaDB</span>
  <span class="tech-badge">VoyageAI</span>
  <span class="tech-badge">Docker</span>
</div>

### Data Science & ML

<div class="tech-stack">
  <span class="tech-badge">pandas</span>
  <span class="tech-badge">NumPy</span>
  <span class="tech-badge">scikit-learn</span>
  <span class="tech-badge">LightGBM</span>
  <span class="tech-badge">XGBoost</span>
  <span class="tech-badge">TensorFlow</span>
  <span class="tech-badge">PyTorch</span>
</div>

### Data Engineering & Visualization

<div class="tech-stack">
  <span class="tech-badge">ETL Pipelines</span>
  <span class="tech-badge">REST APIs</span>
  <span class="tech-badge">Streamlit</span>
  <span class="tech-badge">Plotly</span>
  <span class="tech-badge">Power BI</span>
  <span class="tech-badge">Knowage</span>
</div>

### Cloud & Deployment

<div class="tech-stack">
  <span class="tech-badge">AWS</span>
  <span class="tech-badge">Railway</span>
  <span class="tech-badge">Neon</span>
  <span class="tech-badge">Streamlit Cloud</span>
</div>

</div>

---

<p style="font-size:11px; color: #8b949e;">
Template originally forked from
<a href="https://github.com/evanca/quick-portfolio" style="color: #58a6ff;">evanca</a>
</p>
