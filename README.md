# Vulnerable Identities Recognition Corpus (VIRC) for Hate Speech Analysis

## Content of the repository

```
virc
├── Data
│   ├── annotations_italian_1.json
│   ├── annotations_italian_2.json
│   ├── corpus_italian_1.csv
│   ├── corpus_italian_2.csv
│   │ 
│   ├── annotations_spanish_1.json
│   ├── annotations_spanish_2.json
│   ├── annotations_spanish_disagreement.json
│   ├── corpus_spanish_1.csv
│   ├── corpus_spanish_2.csv
│   ├── corpus_spanish_disagreement.csv
│   │
│   ├── ita_gold.csv
│   └── spa_gold.csv
├── LICENSE
└── README.md
```

- **Data:**
  - `Spanish:` The Spanish data are split into three sets, *1*, *2* and *disagreement*. Sets *1* and *2* contain data annotated by the two original annotators, while the *disagreement* set contains the news where no agreement was reached and a third annotator was needed.
  - `Italian:` The Italian data are divided into two sets (*1* and *2*), annotated by two annotators.
  - `Gold-standard:` The gold-standard dataset generated through the process explained in the paper correspond to the *ita_gold.csv* and *spa_gold.csv* files.
