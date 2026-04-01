# 🌍 Food & Climate AI Agent

> *"I started this project during my Data Analytics Bootcamp in AllWomen last year, but never had time to build the dashboard I envisioned. This is the completion of that story — now powered by AI."*
> — Ivana Caridad Lovera Ruiz

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://food-climate-ai-agent-m6nkzugdffpk3uftxphappk.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)](https://www.python.org/)
[![Claude](https://img.shields.io/badge/Powered%20by-Claude%20AI-orange.svg)](https://www.anthropic.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

---

## 🔗 Live Demo

**[Launch the App →](https://food-climate-ai-agent-m6nkzugdffpk3uftxphappk.streamlit.app/)**

Ask the agent anything:
- *"Which food item has the highest CO2 emissions?"*
- *"Show me data for Brazil"*
- *"Compare Portugal and Spain"*
- *"What is the temperature change trend over the years?"*

---

## 📖 The Story Behind This Project

In 2025, I completed a **Data Analytics Bootcamp** with AllWomen, and built a full data analysis project on food production and climate change — [Food & Climate: Data-Driven Sustainability](https://github.com/ivanya93/Food-Climate-Data-Driven-Sustainability). I always wanted to turn it into an interactive tool but never found the time.

In 2026, while studying my **Master's in Business Analytics & AI at Porto Business School**, I learned to build AI agents. This project is the completion of that original vision — not just a dashboad, but a conversational AI analyst that anyone can query in plain English.

---

## 🤖 What This Agent Does

This is a **conversational AI Data Analyst** built on top of Claude (Anthropic). It can:

- 📊 **Analyze** 101,596 rows of real food & climate data (1961–2022)
- 🌡️ **Answer questions** about CO2 emissions, GHG per kg, temperature change, and food production
- 🌍 **Compare countries** across all metrics
- 🧠 **Remember context** — ask follow-up questions naturally
- 💾 **Export insights** to a text report
- 🔄 **Reason autonomously** — decides which tool to use and loops until the task is complete

---

## 🗂️ Dataset

| Field | Detail |
|---|---|
| **Source** | FAO + Climate Change Data |
| **Rows** | 101,596 |
| **Years** | 1961 – 2022 |
| **Countries** | 202 |
| **Columns** | country, year, food_item, avg_year_temp_change, emissions_CO2eq_AR5, GHG_kg, production_tonnes |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **AI Brain** | Claude Sonnet (Anthropic API) |
| **Agent Framework** | Custom Python agent loop with tool use |
| **Data** | Pandas (101k rows) |
| **Frontend** | Streamlit |
| **Deployment** | Streamlit Community Cloud |
| **Version Control** | GitHub |

---

## 🏗️ Architecture

```
User Question (natural language)
        ↓
   Claude (thinks: what tool do I need?)
        ↓
   Tool selected & executed
   ├── get_dataset_info()
   ├── query_data()
   ├── get_country_data()
   └── compare_countries()
        ↓
   Result returned to Claude
        ↓
   Claude interprets & answers
        ↓
   Follow-up? → Loop continues
        ↓
   Final insight delivered
```

---

## 🚀 Run Locally

```bash
# Clone the repo
git clone https://github.com/ivanya93/food-climate-ai-agent.git
cd food-climate-ai-agent

# Install dependencies
pip install -r requirements.txt

# Add your API key
echo "ANTHROPIC_API_KEY=your-key-here" > .env

# Run the app
streamlit run app.py
```

Or run the terminal version:
```bash
python data_agent.py
```

---

## 📁 Project Structure

```
food-climate-ai-agent/
├── app.py                          # Streamlit web app
├── data_agent.py                   # Terminal agent with memory
├── requirements.txt                # Dependencies
├── final_merged_dataset_Food_Climate_Project.csv  # Dataset
└── .gitignore
```

---

## 🔗 Related Projects

- **[Food & Climate: Data-Driven Sustainability](https://github.com/ivanya93/Food-Climate-Data-Driven-Sustainability)** — The original bootcamp project this agent is built upon. Data cleaning, EDA, and Power BI dashboards.

---

## 👩‍💻 About the Author

**Ivana Caridad Lovera Ruiz**

Data Analyst & AI enthusiast with a background in Accounting & Finance, now specialising in Business Analytics and AI.

- 💼 **Current role:** Data Analyst (Consultant) — Natixis BPCE, Data Management & AI Department via Axco CMG
- 🎓 **Education:** Master in Business Analytics & AI — Porto Business School | Master in Accounting & Finance Management — EAE Business School & Universidad Rey Juan Carlos
- 🛠️ **Tools:** Python · SQL · Power BI · Power Automate · Power Apps · Jira · LLMs · Data Architecture
- 🌍 **Based in:** Porto, Portugal
- 🔗 **LinkedIn:** [linkedin.com/in/ivanacaridadloveraruiz](https://www.linkedin.com/in/ivanacaridadloveraruiz/)

---

## 📄 License

MIT License — feel free to use, adapt, and build on this project.

---

*Built with 🤖 Claude AI + 🐍 Python + ❤️ curiosity*
