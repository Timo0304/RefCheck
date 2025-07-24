# 📚 RefCheckAI: Academic Reference Verification Tool

**RefCheckAI** is a lightweight Streamlit-based tool that verifies the authenticity and metadata of references (citations) in academic documents. It checks for author names, article title, journal name, year of publication, and DOI using trusted sources like **CrossRef**, **PubMed**, and **Semantic Scholar**.

---

## 🔍 Features

- ✅ Upload support for `.csv`, `.docx`, and `.pdf` reference lists
- 🔎 Automatically verifies:
  - Author names
  - Article titles
  - Journal names
  - Year of publication
  - DOI
- 📊 Fuzzy matching for misspelled entries
- 📄 Export verification results to:
  - CSV
  - Word DOCX
  - PDF
- 🌐 Uses APIs from:
  - [CrossRef](https://www.crossref.org/)
  - [PubMed](https://pubmed.ncbi.nlm.nih.gov/)
  - [Semantic Scholar](https://www.semanticscholar.org/)

---

## 🧠 Model & Logic

RefCheckAI uses:

- ✅ **Levenshtein Distance / FuzzyWuzzy** for fuzzy matching
- 🔗 Real-time API queries to fetch metadata for citation verification
- 🧠 Optional GPT integration for natural language feedback on citation quality (coming soon)

---

## 🗂 File Upload Formats

- `CSV`: Each row should contain columns like `Author`, `Title`, `Journal`, `DOI`, `Year`
- `DOCX`: References listed as plain text (one per paragraph or line)
- `PDF`: Extracts text using basic layout parsing (experimental)

---

## 🚀 How to Run Locally

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/RefCheckAI.git
   cd RefCheckAI
