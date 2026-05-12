# 🎓 GO UNI — AI-Powered University Admissions Chatbot

> Verification-first admissions guidance using hybrid retrieval, deterministic eligibility checking, intelligent document analysis and programme recommendation.

**Zina Jalal Samha | Student ID: 23124705**  
BSc Computer Science with Artificial Intelligence  
Birmingham City University | Supervised by Dr Hadeel Saadany  
Module: CMP6200 — Final Year Project

---

## 🎬 Demo Video

[▶ Watch the GO UNI Live Demo](https://1drv.ms/v/c/44a59d0c17339882/IQAdwiOTzpZHQIRuooRhvbCUAQ4f23gWnCp29XfxYPivmqM?e=ggqeab)

---

## 📊 Key Results

| Metric | Result |
|---|---|
| Universities Covered | 4 (BCU, UoB, Aston, Manchester) |
| Programmes Indexed | 77 |
| Evaluation Questions | 75 |
| Answer Accuracy | **100%** |
| Recall@1 / Recall@3 | **100% / 100%** |
| MRR | **1.0000** |
| Synthetic Profiles Tested | 55 |
| Nationalities Covered | 21 |

---

## 🧠 What is GO UNI?

GO UNI is a hybrid RAG (Retrieval-Augmented Generation) admissions assistant that helps prospective students:

- ✅ Check eligibility for university programmes
- 🔍 Explore entry requirements across four UK universities
- 📄 Upload and analyse personal documents (transcripts, certificates)
- 🎯 Receive personalised course recommendations
- 💬 Ask natural language admissions questions with evidence-backed answers

GO UNI is **not** a trained model — it uses pre-trained components (GPT-4o-mini, MiniLM-L6-v2) combined with a structured knowledge base, making its outputs **transparent, traceable and bounded**.

---

## 🏗️ System Architecture

**Three-tab interface:**
- **Chat** — Natural language admissions queries
- **Tools** — Programme search, eligibility checker, document upload
- **History** — Saved conversation sessions

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| Frontend | HTML, CSS, JavaScript |
| LLM | GPT-4o-mini (OpenAI API) |
| Retrieval | BM25 + FAISS (hybrid) |
| Embeddings | MiniLM-L6-v2 (sentence-transformers) |
| Database | SQLite |
| Knowledge Base | CSV datasets |
| Document Parsing | pdfplumber, python-docx |
| Preprocessing | Google Colab |

---

## 📁 Project Structure

---

## ⚙️ Setup & Installation

1. **Clone the repository**
```bash
   git clone https://github.com/itszina/go-uni.git
   cd go-uni
```

2. **Install dependencies**
```bash
   pip install -r requirements.txt
```

3. **Add your OpenAI API key**  
   Create a `.env` file in the root directory:

   4. **Run the application**
```bash
   python app.py
```

5. Open your browser at `http://localhost:5000`

---

## 📓 Research Notebook

The Colab notebook (`notebooks/GO_UNI_FINAL_PROJECT.ipynb`) covers:
- Data preprocessing and knowledge base construction
- BM25 index and FAISS embedding generation
- Evaluation: answer accuracy, retrieval metrics, eligibility testing, recommender pilot
- EDA with 12 standardised figures (Fig_01–Fig_12)

---

## ⚠️ Disclaimer

GO UNI provides **evidence-aware admissions guidance only** — it does not make official admissions decisions. Always verify entry requirements directly with the university.

---

## 📜 References (BCU Harvard)

- Aloqayli and Abdelhafez (2023)
- Okonkwo and Ade-Ibijola (2021)
- Page and Gehlbach (2017)
- UCAS (2025)
- Wollny et al. (2021)

---

*Final Year Project — CMP6200 | Birmingham City University | 2024–2025*
