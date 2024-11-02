# RIRAG: Regulatory Information Retrieval and Answer Generation

### Authors
Azka Basit, Mahnoor Zamir, Mariam Babar, Rameen Aamir  
School of Electrical Engineering and Computer Science (SEECS),  
National University of Sciences & Technology (NUST), Islamabad, Pakistan.

---

## Overview
**RIRAG** aims to enhance regulatory compliance by retrieving relevant passages from complex legal documents and generating accurate responses to regulatory queries using advanced NLP models.

---

## Methodology
1. **Information Retrieval**: Uses the **BM25** algorithm to locate passages most relevant to user queries.
2. **Answer Generation**: Employs **LLaMA** through the **Grok API** to synthesize responses based on retrieved content.

---

## Dataset
The project uses the **ObliQA** dataset, a Regulatory NLP-specific dataset comprising documents from Abu Dhabi Global Markets (ADGM) with numbered clauses and cross-references.

---

## Evaluation Metrics
- **Information Retrieval**: Evaluated using MAP@10 and Recall@10.
- **Answer Generation**: Assessed with RePass (Relevant Passage-based Answer Similarity Score).

---

## Installation and Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/rirag.git
   cd rirag
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API Access**
   ```bash
   GROK_API_KEY=your_api_key_here
   ```

4. **Run the Main Notebook**
   ```bash
   jupyter notebook notebooks/main.ipynb
   ```

---

## Repository Structure
```
regulatory-information-retrieval-and-answer-generation/
├── data/
│   └── input.json       # Input data for queries
├── notebooks/
│   └── main.ipynb       # Main notebook for pipeline execution
├── requirements.txt     # Project dependencies
└── README.md            # Project documentation
```

---

## Usage
Run the notebook to retrieve relevant passages and generate responses. The results are saved in JSON format for further evaluation.

---

## Note
This project is designed to aid regulatory information processing and compliance verification. For questions or contributions, please contact the authors.
