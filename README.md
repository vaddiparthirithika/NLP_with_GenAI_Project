#RAG-Based AI System for Medical Knowledge Retrieval – Merck Manual

##Problem Statement

In the rapidly evolving healthcare industry, professionals often face the challenge of **information overload**. Navigating massive volumes of medical data while making timely, life-critical decisions can be overwhelming. This project proposes a **Retrieval-Augmented Generation (RAG)** based AI system that uses the Merck Medical Manual to deliver **accurate, concise, and grounded responses** to medical queries.

---

##Business Context

- Healthcare providers need **fast, reliable access** to diagnostic and treatment information.
- Traditional methods of looking through manuals and research papers are **time-consuming** and **inefficient**, especially during emergencies.
- A centralized, intelligent retrieval system can **standardize care**, **reduce decision fatigue**, and **improve patient outcomes**.

---

## Objective

Develop a prototype AI system that:
- Uses **RAG architecture** to extract and generate answers from the Merck Manual.
- Addresses real-world medical queries across diagnostics, treatment, drugs, and critical care.
- Demonstrates efficiency and reliability in decision-making support.

---

## Data Description

- **Source**: The Merck Medical Manual (PDF format)
- **Size**: 4,000+ pages
- **Content**: Covers diseases, diagnostics, medications, tests, and treatments
- **Sections**: 23 sections in total

---

##Technologies & Libraries Used

- `PyMuPDF` – PDF text extraction
- `sentence-transformers` – Embedding medical text
- `langchain` – Framework to build the RAG pipeline
- `transformers` – Hugging Face models for generation
- `chromadb` – Vector store for fast similarity search
- `torch`, `tiktoken`, `huggingface_hub`, `langchain_community`

### Observations

- Highly relevant and grounded responses generated from the manual.
- Prompt design plays a critical role in producing structured and accurate answers.
- Default RAG parameters offered the best performance during testing.
- Ideal for clinical and research environments where trust and accuracy are non-negotiable.

### Business Recommendations

- Deploy RAG models in hospitals to support clinical decision-making.
- Use prompt engineering to enhance accuracy for department-specific queries.
- Enable a feedback loop to refine responses based on real-world usage.
- Regularly update vector databases with newer manuals and research data.
- Prioritize models that deliver reliable, context-aware, and grounded responses.

### Files Included
- medical_rag_system.ipynb – Full notebook for PDF ingestion, vectorization, and querying.
- medical_rag_system.html – HTML output for review.
- README.md – Project documentation.
- The Merck Medical Manual (PDF format)

### Future Enhancements
- Add voice support for speech-based querying.
- Deploy a Streamlit UI for ease of use in hospitals.
- Include feedback tracking to refine model performance.
- Integrate multi-modal data (e.g., symptoms + X-ray reports).