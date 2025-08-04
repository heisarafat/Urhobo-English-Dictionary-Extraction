# Urhobo-English Dictionary Corpus Extraction

This project extracts, cleans, and aligns Urhobo-English translation pairs from a scanned PDF dictionary. The goal is to build a high-quality parallel corpus for training machine translation models, as part of the Dala Translate internship Project

## 📘 Description

The source file was a dictionary PDF containing hundreds of Urhobo words with their English equivalents. Many entries were unstructured and required careful extraction using a combination of text processing and regular expressions.

## 🧩 Methodology

- Extracted raw text from PDF using [`pdfplumber`]
- Parsed Urhobo-English pairs with `regex`, handling special characters and tone marks
- Cleaned headers, tone guides, formatting lines, and non-entry sections
- De-duplicated and normalized multi-line or split entries
- Final dataset stored as a structured `.csv` file

## 🛠 Tools Used

- Python
- `pdfplumber`
- `re` (Regex)
- `pandas`
- Google Colab

## 📄 Output

- **File**: `urhobo_english_corpus.csv`
- **Columns**: `urhobo`, `english`
- **Total entries**: 599 aligned translation pairs
- **Format**:

  | urhobo | english |
  |--------|---------|
  | Abe    | A species of water yam with red colored leaves and tuber |
  | Abe    | Guilty verdict |
  | Abo    | Wrestling |
  | Abo    | HANDS - plural form |
  | ...    | ...     |

## 📌 Usage

You can use this CSV as:
- A parallel corpus for machine translation training
- A language dataset for NLP tasks related to Urhobo
- A base for building glossaries or educational tools

## 👤 Author

This project was completed by **[Arafah Ibitoye]** as part of the data extraction task for the Dala Translate internship (August 2025).

---

> For questions or collaboration, feel free to reach out via [arafahibitoye@gmail.com].
