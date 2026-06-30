# Code

Place your implementation files in this folder. Suggested structure based on the BiCEVul pipeline:

```
code/
├── models/
│   ├── encoders.py          # shared dual encoder (CLS pooling)
│   ├── cross_attention.py   # bidirectional cross-attention with alpha gates
│   ├── pooling.py           # sigmoid-gated adaptive multi-scale pooling
│   ├── fusion.py            # hierarchical softmax fusion
│   └── bicevul.py           # full model assembly
├── train.py                 # training entry point
├── evaluate.py               # evaluation / metrics
├── baselines/
│   ├── train_ml.py          # Decision Tree, Random Forest, LR, SVM, XGBoost
│   ├── train_transformers.py # CodeBERT, GraphCodeBERT, CodeT5, UniXcoder, LineVul
│   └── train_llms.py        # CodeLlama-7B, DeepSeek-Coder-7B-Instruct (4-bit NF4 + LoRA)
├── utils/
│   ├── data_loader.py
│   └── metrics.py
└── requirements.txt
```

Update this README with exact run commands once scripts are added (e.g. `python train.py --dataset devign --config configs/bicevul.yaml`).
