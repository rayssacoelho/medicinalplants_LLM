# Medicinal Plants Question Answering with Fine-Tuning and LoRA

## 📌 About the Project

This project implements a complete NLP pipeline for domain adaptation of Large Language Models (LLMs) focused on medicinal plants knowledge.

The objective is to automatically generate an instruction-following dataset from educational documents, fine-tune language models using LoRA (Low-Rank Adaptation), evaluate model performance through NLP metrics, and compare different Seq2Seq and Causal architectures.

The project was developed as part of the Advanced Topics in Artificial Intelligence course and follows the complete workflow of a Retrieval-Augmented Generation (RAG) and Fine-Tuning system.

---

## 📚 Tools Used

This project uses the following technologies:

- Python 3.12+
- PyTorch
- Hugging Face Transformers
- PEFT (LoRA)
- Datasets
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- NLTK
- SacreBLEU
- ROUGE Score
- Google Colab
- Jupyter Notebook

---

## 📂 Project Structure

```bash
medicinalplants_LLM/
│
├── dataset/
│   ├── raw/
│   ├── processed/
│   └── dataset_plantas.jsonl
│
├── models/
│   ├── causal_model_1/
│   ├── causal_model_2/
│   ├── seq2seq_model_1/
│   └── seq2seq_model_2/
│
├── notebooks/
│   ├── 01_dataset_generation.ipynb
│   ├── 02_lora_finetuning.ipynb
│   ├── 03_model_evaluation.ipynb
│   └── main_api.ipynb
│
├── figures/
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🔄 Project Pipeline

The pipeline follows these stages:

### 1. Knowledge Extraction

- PDF document loading
- Text extraction
- Text cleaning
- Chunk generation

### 2. Dataset Generation

- Automatic question generation
- Automatic answer generation
- Instruction tuning format creation
- Dataset curation and validation

### 3. Fine-Tuning

- Dataset preprocessing
- Tokenization
- LoRA configuration
- Parameter-efficient fine-tuning

### 4. Model Evaluation

- Perplexity (PPL)
- BLEU
- ROUGE
- Faithfulness
- Answer Relevance
- Plan Adherence

### 5. Model Comparison

- Seq2Seq models
- Causal models
- Performance comparison
- Best model selection

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/rayssacoelho/medicinalplants_LLM.git
cd medicinalplants_LLM
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate environment

Windows:

```bash
.venv\Scripts\activate
```

Linux/Mac:

```bash
source .venv/bin/activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 Running the Project

### Generate Dataset

```bash
jupyter notebook 01_dataset_generation.ipynb
```

### Fine-Tune Models

```bash
jupyter notebook 02_lora_finetuning.ipynb
```

### Evaluate Models

```bash
jupyter notebook 03_model_evaluation.ipynb
```

---

## 🧠 Models Evaluated

### Seq2Seq Models

- Google FLAN-T5 Base
- MT5 Base

### Causal Models

- Gemma 2 1B
- SmolLM2 1.7B

---

## 📊 Evaluation Metrics

The following metrics were used to assess model quality:

| Metric | Description |
|----------|------------|
| Perplexity | Predictive capability |
| BLEU | N-gram precision |
| ROUGE | Content overlap |
| Faithfulness | Consistency with source knowledge |
| Answer Relevance | Alignment with the question |
| Plan Adherence | Structural similarity to reference |

---

## 📈 Results

### Dataset Statistics

- Generated from medicinal plant educational documents
- Manual quality validation
- Instruction-following format
- Domain-specific knowledge base

### Model Evaluation

Add your final comparison table here:

| Model | PPL | BLEU | ROUGE-L | Faithfulness |
|---------|---------|---------|---------|---------|
| Model 1 | - | - | - | - |
| Model 2 | - | - | - | - |
| Model 3 | - | - | - | - |
| Model 4 | - | - | - | - |

---

## 🌿 Example Question

**Question**

```text
What are the medicinal properties of rosemary?
```

**Expected Answer**

```text
Rosemary is commonly used for digestive problems,
circulation improvement, and anti-inflammatory effects.
```

---

## 🎯 Key Learnings

- Instruction Dataset Generation
- Domain Adaptation of LLMs
- Parameter-Efficient Fine-Tuning (PEFT)
- LoRA Optimization
- NLP Evaluation Metrics
- Hugging Face Ecosystem
- Model Comparison and Benchmarking

---

## 👨‍💻 Author

**Rayssa Coelho Silva**

Computer Science Student – UFRN

Advanced Topics in Artificial Intelligence

2026
