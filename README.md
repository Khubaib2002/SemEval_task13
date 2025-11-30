# SemEval-2026 Task 13: Machine-Generated Code Detection
## Sub Task A Description

Given a code snippet, classify whether it was:
- **Human-written (0)**: authored by a Human
- **Machine-generated (1)**: produced by an AI/LLM

## Project Structure

```
code/
├── approaches/
│   ├── baseline           # contains the baseline ipnyb file
│   ├── ensemble           # contains the ensemble approach using GraphCodeBERT and CodeBERT ipnyb file
├── final_submission.csv
└── README.md
```

## Quick Start

### 1. Clone the Repository
### 2. Choose an Approach
- Baseline
- Ensemble

### 3. Run the Jupyter Notebook files

## Dataset

The dataset is from the [SemEval-2026 Task 13](https://semeval.github.io/) shared task and is available on HuggingFace.

### Download Data using HuggingFace Datasets**
```python
from datasets import load_dataset
ds = load_dataset("DaniilOr/SemEval-2026-Task13", "A")
```

### Data Format

| Column | Description |
|--------|-------------|
| `code` | Source code string |
| `label` | 0 (human) or 1 (machine) |
| `language` | Programming language |
| `generator` | Source of the code |
