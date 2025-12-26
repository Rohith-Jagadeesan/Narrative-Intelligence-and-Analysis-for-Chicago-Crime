# Narrative Intelligence for Urban Crime Analysis

## Overview
Urban crime analysis often relies on machine learning models that deliver accurate predictions but provide limited interpretability for policymakers, researchers, and communities. This project introduces a **Hybrid Retrieval-Augmented Generation (RAG) system** that transforms large-scale, structured crime data into **contextual, human-readable narratives**.

Using **Chicago Police Department crime records (2018–2025)** and **Chicago Tribune news articles**, the system combines traditional predictive modeling with semantic retrieval and large language model synthesis to explain **not just what is happening, but why it is happening**. The result is a narrative intelligence framework that bridges the gap between predictive accuracy and real-world understanding.


## Key Contributions
- Demonstrates limitations of traditional ML models (Logistic Regression, Random Forest, XGBoost) in explaining crime patterns despite high accuracy.
- Builds a hybrid RAG pipeline combining **semantic embeddings, FAISS indexing, deterministic crime–news linking, and LLM-based synthesis**.
- Generates evidence-grounded narratives that contextualize crime trends across time, space, and media coverage.
- Evaluates narrative quality using retrieval, faithfulness, and context-utilization metrics.


## System Architecture
**Pipeline Summary:**
1. **Data Ingestion**  
   - Chicago crime records (1.88M incidents)  
   - Chicago Tribune news articles (~15K articles)

2. **Preprocessing & Chunking**  
   - Temporal, spatial, and crime-type segmentation  
   - 92% compression into semantic chunks

3. **Embedding & Indexing**  
   - SentenceTransformer embeddings  
   - FAISS vector indices for efficient retrieval

4. **Deterministic Linking Engine**  
   - High-confidence crime–news connections using time, keyword, and location filters

5. **Hybrid Retrieval**  
   - Semantic similarity + deterministic links  
   - Crime- and news-aware retrieval

6. **LLM Synthesis**  
   - Google Gemini generates grounded, narrative explanations



## Evaluation Highlights
- **Average documents retrieved:** 8.7  
- **Average faithfulness:** 78.3%  
- **Average context utilization:** 52.5%  
- **Overall RAG performance score:** **83.84%**  
- **Hallucination reduction:** ~80% compared to LLM-only baselines

The hybrid RAG approach significantly outperforms keyword search, embeddings-only retrieval, and zero-shot LLM generation.


## Why This Matters
Crime analytics should not stop at prediction. Policymakers, community leaders, journalists, and researchers need explanations they can trust and act upon.

This project:
- Translates complex statistical outputs into **interpretable narratives**
- Reduces hallucinations through evidence-grounded generation
- Enables better decision-making by linking crime patterns to real-world context
- Demonstrates how **narrative intelligence** can make AI systems more transparent and socially useful

The frontier of urban analytics is not higher accuracy alone—but **better communication of insights**.


## Technologies Used
- Python, Pandas, NumPy  
- SentenceTransformers  
- FAISS  
- Scikit-learn, XGBoost  
- Google Gemini API  
- Jupyter Notebook


## License
This project is released for academic and research use.
