# 🧊 POLAR: Polarization Detection in Social Media

**Developed for the NLP-2026 Lecture by Team 13**

## 📖 What We Are Doing
The **POLAR** project addresses a critical challenge in modern computational linguistics: **identifying and classifying polarization in social media posts and comments**. 

As digital discourse becomes increasingly divided, understanding the nuance of polarized language is essential. This repository holds our comprehensive NLP pipeline to scrape, clean, process, and classify social media texts using state-of-the-art Transformer architectures. 

We break this problem down into two primary tracks:
*   **Task 1:** Baseline polarization identification (e.g., detecting if a post contains polarized or neutral language).
*   **Task 2:** Granular classification (e.g., evaluating the degree, specific stance, or target of the polarization).

## 🧠 Models & Methodology
We evaluate and benchmark three leading Transformer architectures to see which handles the semantic complexity and informal structure of social media text best:
1.  **BERT** (Bidirectional Encoder Representations from Transformers): Tested and evaluated on both Task 1 and Task 2.
2.  **RoBERTa** (Robustly Optimized BERT Pretraining Approach): Tested and evaluated on both Task 1 and Task 2, leveraging its larger pre-training corpus and dynamic masking.
3.  **DeBERTa** (Decoding-enhanced BERT with Disentangled Attention): Directly benchmarked against RoBERTa specifically for Task 2 to evaluate if its disentangled attention mechanism improves nuance detection.

## 📂 Repository Structure

### Core Code
*   [`POLAR_code.ipynb`](./POLAR_code.ipynb): The main execution pipeline containing data preprocessing, model initialization, and training loops for BERT and RoBERTa on both tasks.
*   [`POLAR_deberta_test.ipynb`](./POLAR_deberta_test.ipynb): A dedicated testing environment isolating Task 2, pitting DeBERTa against RoBERTa.

### Documentation & Reports
*   [`POLAR_report.pdf`](./POLAR_report.pdf) & `Polar.pdf`: The official Team 13 project reports detailing our theoretical approach, hyperparameters, metrics, and final conclusions.

### Visualizations & Results
*   `POLAR.png`: High-level overview of our architecture and final working results.
*   `Train_val_loss_Bert_task_1.png` & `Train_val_loss_Bert_task_2.png`: Training vs. Validation loss curves for BERT across both tasks.
*   `Train_val_loss_Roberta_task_1.png` & `Train_val_loss_Roberta_task_2.png`: Training vs. Validation loss curves for RoBERTa across both tasks.

## ⚙️ Prerequisites & Setup
To run these notebooks, you will need a Python environment equipped for Deep Learning. We recommend using `conda` or a standard virtual environment (`venv`).

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/saad-rahman25/POLAR.git](https://github.com/saad-rahman25/POLAR.git)
   cd POLAR
