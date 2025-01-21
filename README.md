# Vulnerable Identities Recognition Corpus (VIRC) for Hate Speech Analysis
Welcome to the Vulnerable Identities Recognition Corpus (VIRC), a dataset created to enhance hate speech analysis in Italian and Spanish news headlines. VIRC provides annotated headlines aimed at identifying vulnerable identities, dangerous discourse, derogatory mentions, and entities. This corpus contributes to developing more sophisticated hate speech detection tools and policies for creating a safer online environment.

## Overview

VIRC is designed to support the study of hate speech in headlines from two languages: Italian and Spanish. It includes 880 headlines (532 Italian and 348 Spanish), collected and annotated with the following labels:
- *Named Entities*: Identifies persons, locations, organizations, groups, etc. mentioned in the headline.
- *Vulnerable Identity Mentions*: Labels groups such as women, LGBTQI, ethnic minorities, and migrants targeted by hate speech.
- *Derogatory Mentions*: Marks phrases that are derogatory towards vulnerable groups.
- *Dangerous Speech*: Highlights parts of the text perceived as potentially inciting hate or perpetuating harmful stereotypes.

## Content of the Project
```
virc
├── Data
│   ├── annotations_italian_1.json
│   ├── annotations_italian_2.json
│   ├── corpus_italian_1.csv
│   ├── corpus_italian_2.csv
│   │ 
│   ├── annotations_spanish_1.json
│   ├── annotations_spanish_2.json
│   ├── annotations_spanish_disagreement.json
│   ├── corpus_spanish_1.csv
│   ├── corpus_spanish_2.csv
│   ├── corpus_spanish_disagreement.csv
│   │
│   ├── ita_gold.csv
│   └── spa_gold.csv
│  
├── VIRC_Guidelines.pdf
├── VIRC.ipynb
├── LICENSE
├── CITATION.cff
└── README.md
```

## Annotation
The `VIRC_Guidelines.pdf` contains the annotation guidelines provided to annotators. This can be seen sintetized in the paper.

## Data
- *Spanish*: The Spanish datasets are split into two sets, agreement and disagreement. Agreement set contains the data annotated by the two original annotators, while the disagreement set contains the news where no agreement was reached and a third annotator was needed
- *Italian*: The Italian data consists of only one set annotated by two annotators.

## Usage
The dataset has been uploaded to Hugging Face. You can access the dataset and its documentation at the following repository: [https://huggingface.co/datasets/oeg/virc](https://huggingface.co/datasets/oeg/virc).

## Jupyter Notebook

The `VIRC.ipynb` notebook contains all the code for the generation of the gold-standard dataset, calculation of the F-scores, statistics mentioned in the paper and the zero shot experiments. 

### Required Files
To ensure the notebook runs correctly, the following files are required. Please reach out to the authors to obtain them:
- `annotations_italian_1.json`
- `annotations_italian_2.json`
- `corpus_italian_1.csv`
- `corpus_italian_2.csv`
- `annotations_spanish_1.json`
- `annotations_spanish_2.json`
- `annotations_spanish_disagreement.json`
- `corpus_spanish_1.csv`
- `corpus_spanish_2.csv`
- `corpus_spanish_disagreement.csv`
- `ita_gold.csv`
- `spa_gold.csv`

### Python Requirements
Ensure the following Python packages are installed:
``` python
tqdm==4.64.1
transformers==4.36.2
torch==2.1.2
pandas==1.4.4
```
## Cite
``` bibtex


@inproceedings{IbaiArianna2024,
  author       = {Ibai Guill{\'{e}}n{-}Pacho and
                  Arianna Longo and
                  Marco Antonio Stranisci and
                  Viviana Patti and
                  Carlos Badenes{-}Olmedo},
  editor       = {Felice Dell'Orletta and
                  Alessandro Lenci and
                  Simonetta Montemagni and
                  Rachele Sprugnoli},
  title        = {The Vulnerable Identities Recognition Corpus {(VIRC)} for Hate Speech
                  Analysis},
  booktitle    = {Proceedings of the Tenth Italian Conference on Computational Linguistics
                  (CLiC-it 2024), Pisa, Italy, December 4-6, 2024},
  series       = {{CEUR} Workshop Proceedings},
  volume       = {3878},
  publisher    = {CEUR-WS.org},
  year         = {2024},
  url          = {https://ceur-ws.org/Vol-3878/49_main_long.pdf},
}
```

## Contact
You can contact us through our email adresses:
- ibai.guillen@upm.es
- arianna.longo401@edu.unito.it
- marcoantonio.stranisci@unito.it
- viviana.patti@unito.it
- carlos.badenes@upm.es.

## Acknowledgements
This work is supported by the Predoctoral Grant (PIPF-2022/COM-25947) of the Consejería de Educación, Ciencia y Universidades de la Comunidad de Madrid, Spain. Arianna Longo's work has been supported by aequa-tech.
The authors gratefully acknowledge the Universidad Politécnica de Madrid (www.upm.es) for providing computing resources on the IPTC-AI innovation Space AI Supercomputing Cluster.

## License
This work is licensed under the MIT License. For more details, see the LICENSE file.
