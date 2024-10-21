# Vulnerable Identities Recognition Corpus (VIRC) for Hate Speech Analysis
Welcome to the Vulnerable Identities Recognition Corpus (VIRC), a dataset created to enhance hate speech analysis in Italian and Spanish news headlines. VIRC provides annotated headlines aimed at identifying vulnerable identities, dangerous discourse, derogatory mentions, and entities. This corpus contributes to developing more sophisticated hate speech detection tools and policies for creating a safer online environment.

## Overview

VIRC is designed to support the study of hate speech in headlines from two languages: Italian and Spanish. It includes 880 headlines (532 Italian and 348 Spanish), collected and annotated with the following labels:
- Named Entities: Identifies persons, locations, organizations, groups, etc. mentioned in the headline.
- Vulnerable Identity Mentions: Labels groups such as women, LGBTQI, ethnic minorities, and migrants targeted by hate speech.
- Derogatory Mentions: Marks phrases that are derogatory towards vulnerable groups.
- Dangerous Speech: Highlights parts of the text perceived as potentially inciting hate or perpetuating harmful stereotypes.


## Content of the Project

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
│  
├── VIRC.ipynb
├── LICENSE
└── README.md
```

## Data
  - `Spanish:` The Spanish datasets are split into three sets, *1*, *2* and *disagreement*. Sets *1* and *2* contain data annotated by the two original annotators, while the *disagreement* set contains the news where no agreement was reached and a third annotator was needed.
  - `Italian:` The Italian data are divided into two sets (*1* and *2*), annotated by two annotators.
  - `Disaggregated:` The files containing all the annotations are named according to the following schema *annotations_{language}_{set}.json*.
  - `Gold-standard:` The gold-standard dataset generated through the process explained in the paper correspond to the *ita_gold.csv* and *spa_gold.csv* files.

## Jupyter Notebook

The `VIRC.ipynb` notebook contains all the code for the generation of the gold-standard dataset, calculation of the F-scores, statistics mentioned in the paper and the zero shot experiments.


## Contact
You can contact me through my email adress ibai.guillen@upm.es.

## Acknowledgements
This work is supported by the Predoctoral Grant (PIPF-2022/COM-25947) of the Consejería de Educación, Ciencia y Universidades de la Comunidad de Madrid, Spain. Arianna Longo's work has been supported by aequa-tech.
The authors gratefully acknowledge the Universidad Politécnica de Madrid (www.upm.es) for providing computing resources on the IPTC-AI innovation Space AI Supercomputing Cluster.

## License
This work is licensed under the MIT License. For more details, see the LICENSE file.