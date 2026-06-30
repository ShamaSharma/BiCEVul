# Data

BiCEVul is evaluated on three benchmark datasets: **Devign**, **Reveal**, and **TrVD**, using the publicly available LLM-augmented versions (code paired with GPT-4 generated explanations).

## Download

The datasets are available at:
https://drive.google.com/file/d/1EU3wztfOpmbQdvZoMDAqtnvSEmLT1iL9/view?usp=sharing

## Setup

1. Download the archive from the link above.
2. Extract it into this `data/` directory.
3. Expected structure after extraction:

```
data/
├── devign/
│   ├── train.jsonl
│   ├── valid.jsonl
│   └── test.jsonl
├── reveal/
│   ├── train.jsonl
│   ├── valid.jsonl
│   └── test.jsonl
└── trvd/
    ├── train.jsonl
    ├── valid.jsonl
    └── test.jsonl
```

Each example contains the source code function, its label (vulnerable / safe), and the corresponding LLM-generated explanation.

Note: raw data files are excluded from version control via `.gitignore`. Only this README and any small metadata files should be committed.
