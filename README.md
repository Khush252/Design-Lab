# Chain-of-Thought Enhanced Visual Question Answering using GPT-2

This project demonstrates a prototype for **Chain-of-Thought (CoT) prompting** to improve reasoning in **Visual Question Answering (VQA)** tasks, using **GPT-2** as the backbone model.

The goal was to design a pipeline where questions about images are answered via logical reasoning steps followed by a final answer, showing a structured thought process.

---

## ✨ Project Highlights

- **Model:** GPT-2 Medium (345M parameters)
- **Technique:** Chain-of-Thought (CoT) prompting
- **Training:** Small dataset, limited epochs due to Colab constraints
- **Evaluation Metrics:** Exact Match (EM), BLEU, ROUGE

---

## 📈 Results

| Metric                | Direct Prompting | CoT Prompting |
|------------------------|:----------------:|:-------------:|
| Exact Match (Accuracy) | 0.0000            | 0.0000        |
| BLEU Score             | 0.000078          | 0.000426      |
| ROUGE-1 F1             | 0.002348          | 0.006029      |
| ROUGE-L F1             | 0.002348          | 0.006029      |

🔵 Slight improvement observed using CoT prompting even with very limited fine-tuning.

---

## 🏗️ Project Structure

```bash
├── cot_vqa_gpt2_colab.ipynb   # Main notebook (Colab friendly)
├── report/                    
│    └── final_project_report.pdf   # Detailed written project report
├── README.md                  # Project documentation
└── requirements.txt           # Required Python packages
```

How to Run
Clone this repository or download the notebook.

Install required libraries:
pip install transformers datasets nltk rouge-score
Open cot_vqa_gpt2_colab.ipynb and run all cells sequentially.
