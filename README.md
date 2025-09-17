# Abstractive Summarization of Legal Case Documents

This project focuses on building an abstractive summarization system tailored for legal case documents. It leverages **BART**, a transformer-based sequence-to-sequence model, fine-tuned with **Mean Cosine Similarity (MCS)** chunking to effectively handle long legal texts.

---

## Overview
Legal case documents are often lengthy and complex, making it challenging for lawyers, researchers, and other professionals to quickly grasp their content. This project fine-tunes BART to generate concise and meaningful summaries while maintaining legal context and accuracy.

---

## Key Features
- **Model:** Fine-tuned **BART** for legal text summarization.
- **Chunking Strategy:** **Mean Cosine Similarity (MCS)** to segment long documents.
- **Evaluation Metric:** Achieved **ROUGE-L score of 0.32** on the legal case summarization dataset.
- **Workflow:**  
  1. **Data Preparation:** Cleaning, preprocessing, and chunking of legal cases.  
  2. **Model Fine-Tuning:** BART fine-tuning on chunked data.  
  3. **Evaluation:** Performance measured using ROUGE metrics.

---

## Project Structure
```

ABSTRACTIVE-SUMMARIZATION-OF-LEGAL-CASE-DOCUMENTS/
│
├── data/                               # Dataset files
│   └── Fine\_Tuned\_Data\_FD\_IN-Abs\_CSM\_512.xlsx
│
├── notebooks/                          # Jupyter notebooks
│   ├── 1\_data\_preparation.ipynb        # Data preparation and chunking
│   ├── 2\_model-finetuning.ipynb        # BART fine-tuning
│   └── 3\_evaluation.ipynb              # Model evaluation and analysis
│
├── Court\_case\_summarization\_using\_BART # Core implementation script (if applicable)
├── .gitignore                          # Ignored files
├── kaggle.json                         # Kaggle API credentials (if used for dataset)
└── README.md                           # Project documentation

````

---
Key libraries:

* `transformers`
* `torch`
* `datasets`
* `scikit-learn`
* `pandas`
* `numpy`

---

## Usage

1. **Data Preparation:**
   Run `1_data_preparation.ipynb` to clean and chunk the dataset.

2. **Model Fine-Tuning:**
   Use `2_model-finetuning.ipynb` to fine-tune BART on prepared data.

3. **Evaluation:**
   Evaluate the model using `3_evaluation.ipynb` and check ROUGE scores.

---

## Results

* **ROUGE-L:** 0.32
* Summaries generated are concise while retaining critical legal context.

---

