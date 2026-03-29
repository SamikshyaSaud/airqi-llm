# 🌬️ AirQI-LLM: Air Quality Analysis System

An intelligent Air Quality Analysis Tool that combines **Machine Learning** and 
**Large Language Models (LLMs)** via a **Retrieval-Augmented Generation (RAG)** 
architecture to predict AQI and explain air quality in plain language.

---

## 📌 Features
- 🔢 Predict Air Quality Index (AQI) using ML models
- 🤖 AI-powered chatbot for natural language air quality queries
- 📊 Pollutant trend visualization
- 🏥 Health-based recommendations
- 📁 Upload your own CSV dataset

---

## 🗂️ Project Structure
```
airqi-llm/
│
├── data/                    # Dataset files (CSV)
├── knowledge_base/          # .md and .txt knowledge files for RAG
├── models/                  # Saved ML models
├── notebooks/               # Jupyter notebooks
├── src/
│   ├── ml_pipeline.py       # ML training and prediction
│   ├── rag_pipeline.py      # RAG + ChromaDB setup
│   └── app.py               # Streamlit/Gradio UI
├── requirements.txt
└── README.md
```

---

## 🧠 System Architecture

**RAG Pipeline:**
User Query → Retriever → ChromaDB → LLM → Natural Language Response

**ML Pipeline:**
Dataset → Preprocessing → Model Training → AQI Prediction

---

## 📊 ML Models Used
| Model | Type |
|-------|------|
| Linear Regression | Baseline |
| Random Forest Regressor | Primary |
| Gradient Boosting Regressor | Primary |

**Evaluation Metrics:** MAE, MSE, R² Score

---

## 🧪 Key Pollutants Analyzed
- PM2.5, PM10
- NO₂, SO₂
- CO, O₃

---

## 🛠️ Technologies Used
| Category | Tools |
|----------|-------|
| Language | Python |
| ML | Scikit-learn, Pandas, NumPy |
| LLM | LLaMA / GPT via LangChain |
| Vector Store | ChromaDB |
| Embeddings | HuggingFace |
| UI | Streamlit / Gradio |

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/airqi-llm.git
cd airqi-llm
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the app
```bash
streamlit run src/app.py
```

---

## 📁 Data Source
- [US EPA Air Quality Data](https://www.epa.gov/outdoor-air-quality-data)
- [AQI Basics](https://www.airnow.gov/aqi/aqi-basics)

---

## 🔮 Future Plans
- [ ] Real-time AQI API integration
- [ ] Chat memory / persistent history
- [ ] Cloud deployment
- [ ] Web & mobile app

---

## 👩‍💻 Author
**Samikshya Saud**

---

## 📜 License
MIT License
```

---

## 5. 📁 Suggested Folder Structure to Upload
```
airqi-llm/
│
├── data/
│   └── us_air_quality_sample.csv
├── knowledge_base/
│   ├── aqi_standards.md
│   ├── health_impacts.md
│   └── pollutant_info.txt
├── models/
│   └── trained_model.pkl
├── notebooks/
│   └── airqi_analysis.ipynb
├── src/
│   ├── ml_pipeline.py
│   ├── rag_pipeline.py
│   └── app.py
├── .gitignore
├── requirements.txt
└── README.md
```

---

## 6. 📦 requirements.txt Content
```
pandas
numpy
scikit-learn
langchain
chromadb
streamlit
gradio
huggingface-hub
sentence-transformers
```

---

## 7. 🚫 .gitignore Content
```
__pycache__/
*.pyc
.env
*.pkl
chroma_db/
.ipynb_checkpoints/
venv/
*.csv
