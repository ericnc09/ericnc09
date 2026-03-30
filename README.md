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
* **Published researcher** in medical AI: [CervixCan-Net](https://www.mecs-press.org/ijisa/ijisa-v17-n6/v17n6-10.html) - cervical cancer classification using deep learning
* **Pulished in Big Data Research** [OL-Heatmap](https://doi.org/10.1016/j.bdr.2021.100235) - novel density visualization method
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

### Smart Money Follows — Insider & Congressional Trade Signal Platform
Automated system that tracks what corporate insiders and Congress are trading, scores each signal for conviction, and surfaces the highest-quality opportunities through a live dashboard:
* **Problem:** Insider and congressional trade disclosures are public, but scattered across SEC filings and government reports — buried in XML and HTML. By the time retail investors notice, the edge is gone.
* **Solution:** End-to-end pipeline that ingests trades from SEC EDGAR (Form 4) and Capitol Trades, enriches them with real-time fundamentals and macroeconomic context, and produces a 0–100% conviction score per signal.
* **Scoring model:** Multi-factor conviction engine combining three dimensions:

| Dimension | Weight | Factors |
|---|---|---|
| Signal Strength | 40% | Actor reputation, trade size, insider clustering, disclosure timing, cross-source consensus |
| Fundamental Quality | 35% | Valuation (P/E), momentum, volatility regime (RSI), drawdown opportunity, liquidity |
| Macro Regime | 25% | Yield curve, unemployment, CPI, fed funds rate → Expansion/Transition/Recession modifier (0.5x–1.5x) |

* **Key features:** Direction-aware scoring (buy-the-dip vs sell-at-highs), macro regime detection via FRED, real-time React dashboard with signal table, macro gauge, and conviction breakdowns
* **Data sources:** SEC EDGAR RSS + XML parsing, Capitol Trades RSC scraping, Tiingo API (fundamentals), FRED API (macro) — all zero-cost
* **Tech:** Python, FastAPI, SQLAlchemy, httpx (async), React 18, TypeScript, Vite, Recharts
* **Repo:** [financial-planner](https://github.com/ericnc09/financial-planner)

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
