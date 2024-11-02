# RIRAG: Regulatory Information Retrieval and Answer Generation

### Authors
Azka Basit, Mahnoor Zamir, Mariam Babar, Rameen Aamir  
School of Electrical Engineering and Computer Science (SEECS),  
National University of Sciences & Technology (NUST), Islamabad, Pakistan.

---

## Table of Contents
- [Problem Statement](#problem-statement)
- [Methodology](#methodology)
  - [Information Extraction using BM25](#information-extraction-using-bm25)
  - [Answer Generation using LLaMA](#answer-generation-using-llama)
- [Dataset Overview](#dataset-overview)
- [Evaluation Metrics](#evaluation-metrics)
  - [Information Retrieval Metrics](#information-retrieval-metrics)
  - [Answer Generation Metrics](#answer-generation-metrics)
- [Results](#results)
- [Discussions](#discussions)

---

## Problem Statement
Regulatory compliance is essential for industries, as organizations must adhere to obligations found in lengthy regulatory documents. These documents contain complex legal language, inconsistent formatting, and unstructured content, which poses significant challenges for traditional information retrieval (IR) and question-answering (QA) systems. This project aims to tackle these challenges by developing a system that retrieves pertinent paragraphs and generates precise responses based on the retrieved content.

---

## Methodology
Our methodology employs a two-phase approach to efficiently retrieve information and generate accurate responses to user queries.

### Information Extraction using BM25
The **BM25** ranking function is used to retrieve relevant passages from regulatory documents. BM25 assigns a score to each passage based on its relevance to a given query, effectively filtering a large collection of documents to find the most pertinent sections for further processing.

### Answer Generation using LLaMA
The **LLaMA** model, a robust transformer-based language model, is used to generate accurate responses. After the relevant passages are identified by BM25, LLaMA synthesizes the information to produce a clear, informative response that directly answers the user’s query.

---

## Dataset Overview
The dataset used in this project is the **ObliQA** dataset, specifically designed for Regulatory Natural Language Processing (RegNLP). It includes structured documents from Abu Dhabi Global Markets (ADGM) with numbered clauses and cross-references, facilitating compliance applications in financial services.

- **Total Documents:** 40
- **Document Length:** 30-100 pages each
- **Total Words:** 640,000
- **Dataset Split:** Train (22,295 pairs), Test (2,786 pairs), Development (2,888 pairs)

---

## Evaluation Metrics

### Information Retrieval Metrics
- **MAP@10 (Mean Average Precision at 10):** Measures the precision of the top 10 retrieved passages, accounting for both ranking and relevancy.
- **Recall@10:** The percentage of relevant documents found in the top 10 results for each query.

### Answer Generation Metrics
- **RePass (Relevant Passage-based Answer Similarity Score):** Assesses the accuracy and relevance of generated answers by measuring the semantic similarity between generated answers and relevant passages.

---

## Results

---

## Discussions

---
