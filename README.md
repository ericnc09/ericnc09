# Hi, I'm Eric 👋

I build AI-powered products and ship production systems that solve real problems — and I apply ML research to football data on the side.

Most of my work is hands-on: designing RAG architectures, optimizing LLM performance, and turning messy technical requirements into working products that people actually use.

I recently shipped the **3GPP RAG Assistant** — a production conversational agent serving 15+ telecom engineers that achieved 80% retrieval accuracy and 650% user growth through systematic prompt engineering and iterative optimization.

## What I work on

**AI Agent Development:**
* Production RAG systems: semantic search, retrieval optimization, grounding strategies
* Prompt engineering: systematic A/B testing, performance evaluation, hallucination prevention
* LLM-powered workflows: query routing, context management, latency optimization (<2s response times)
* Conversational interfaces: user-facing agents that handle complex domain-specific queries

**ML Research & Graph Learning:**
* Graph Neural Networks (GCN, GAT) on spatial event data
* Cross-domain generalization: training on one dataset, evaluating on a structurally different one
* Benchmarking GNN models against statistical and industry baselines
* End-to-end pipelines: raw event data → graph construction → model training → evaluation

**Product Development:**
* 0→1 product building: from user research → requirements → MVP → iteration
* AI integration into enterprise workflows: automation, forecasting, operational efficiency
* Data-driven optimization: dashboards, A/B testing, metrics-driven decision making
* Cross-functional execution: working with engineering, operations, and business stakeholders

**Technical Stack:**
* LLMs: OpenAI, Anthropic Claude, RAG architectures
* ML/Deep Learning: PyTorch, PyTorch Geometric, GCN, GAT, scikit-learn
* Languages: Python, SQL
* Tools: PowerBI, Tableau, Git, AI coding assistants
* Frameworks: Agile/Scrum, RICE prioritization, user-centered design

## About Me

* **Product Manager at Rogers Communications** building AI-powered digital products and leading technical initiatives across a $35.6M portfolio
* **MS in Computer Science** (AI & Data Science) from York University — deep learning, machine learning, data visualization
* **Published researcher** in medical AI: CervixCan-Net (cervical cancer classification using deep learning)
* **Engineering background** (4 years): built and shipped 120+ infrastructure projects, worked with cross-functional teams at scale

## Recent Projects

### 3GPP RAG Assistant
Production AI agent for technical documentation retrieval:
* **Problem:** Telecom engineers spending hours searching through 1000+ page 3GPP specifications
* **Solution:** RAG-based conversational agent with semantic search and intelligent query routing
* **Impact:** 80% accuracy, <2s response time, 650% user growth (2 → 15 users)
* **Tech:** LLM-powered retrieval, prompt engineering, performance optimization, user feedback loops

### Football GNN Analysis — Graph Neural Networks on Spatial Football Data
Research pipeline applying GCN and GAT models to football (soccer) data across 6 experiments:
* **Problem:** Can a model learn football tactics and shot quality from player positions alone — without hard-coded rules?
* **Approach:** Players modeled as graph nodes, spatial relationships as edges (Delaunay triangulation). Trained on StatsBomb 360 freeze-frames and Metrica optical tracking data.
* **Results across 6 experiments:**

| Task | Best GNN AUC | Baseline | Takeaway |
|---|---|---|---|
| Team classifier (in-game) | **1.000** (GAT) | 0.547 | GAT perfectly separates formations via edge attention |
| Team classifier (cross-match) | **1.000** (GCN) | 0.547 | GCN generalizes better; classic bias-variance reversal |
| Pass completion (in-competition) | **0.609** (GCN) | ~0.5 | AUC consistent with professional xP models |
| Pass completion (cross-competition, WC2022 → WWC2023) | **0.672** (GAT) | ~0.5 | Spatial geometry transfers across men's & women's football |
| xG model (in-competition) | 0.593 (GAT) | 0.799 LogReg | Distance dominates at this data scale |
| xG model (cross-competition) | 0.603 (GCN) | 0.764 LogReg | GCN beats GAT cross-domain; geometry transfers |

* **Scale:** 107K+ pass-completion graphs · 3,000+ shot graphs · 4 datasets · WC2022 + WWC2023
* **Tech:** PyTorch Geometric, GCNConv, GATv2Conv, StatsBomb Open Data, statsbombpy
* **Repo:** [football-analysis](https://github.com/ericnc09/football-analysis)

### AI Automation at Rogers
Internal tool for operational efficiency:
* **Impact:** 2% operational cost reduction, 40% faster onboarding time
* **Approach:** ML opportunity evaluation, process automation, stakeholder alignment

### ML Forecasting & Analytics
Enterprise-scale data products:
* **Built:** PowerBI/SQL dashboards improving operational visibility by 40%
* **Evaluated:** ML opportunities in network forecasting enabling 15% YoY efficiency gains

## Publications

* **CervixCan-Net: An Enhanced Cervical Cancer Classification Approach using Deep Learning** — IJISA, 2025
* **OL-HeatMap: Effective Density Visualization of Multiple Overlapping Rectangles** — Elsevier Big Data Research, 2021

## How I Work

* **Ship fast, iterate faster:** Built 3GPP MVP in 4 weeks (vs 12-week estimate) through ruthless prioritization
* **User-first:** Conducted research with 10+ stakeholders, created personas, validated through feedback loops
* **Data-driven:** Every decision backed by metrics — A/B testing, performance tracking, continuous optimization
* **Technical depth meets product thinking:** Engineering background enables better collaboration with dev teams and smarter technical tradeoffs

## Let's Connect

🌱 **Building AI products or exploring sports analytics?** I'm always interested in chatting about RAG architectures, LLM optimization, GNN research, or product strategy for AI-powered systems.

📍 Based in Toronto/Hamilton, ON
💼 Open to product roles in AI/ML
📧 ericcosta.public@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/ericcostanil)

---

*I believe the best AI products combine deep technical understanding with relentless focus on user outcomes. Technology should solve real problems, not just showcase capabilities.*
