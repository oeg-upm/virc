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
## BibTeX Entry and Citation Info
``` bibtex
@inproceedings{guillen-pacho-etal-2024-vulnerable,
    title = "The Vulnerable Identities Recognition Corpus ({VIRC}) for Hate Speech Analysis",
    author = "Guill{\'e}n-Pacho, Ibai  and
      Longo, Arianna  and
      Stranisci, Marco Antonio  and
      Patti, Viviana  and
      Badenes-Olmedo, Carlos",
    editor = "Dell'Orletta, Felice  and
      Lenci, Alessandro  and
      Montemagni, Simonetta  and
      Sprugnoli, Rachele",
    booktitle = "Proceedings of the 10th Italian Conference on Computational Linguistics (CLiC-it 2024)",
    month = dec,
    year = "2024",
    address = "Pisa, Italy",
    publisher = "CEUR Workshop Proceedings",
    url = "https://aclanthology.org/2024.clicit-1.50/",
    pages = "417--424",
    ISBN = "979-12-210-7060-6",
    abstract = "This paper presents the Vulnerable Identities Recognition Corpus (VIRC), a novel resource designed to enhance hate speech analysis in Italian and Spanish news headlines. VIRC comprises 921 headlines, manually annotated for vulnerable identities, dangerous discourse, derogatory expressions, and entities. Our experiments reveal that large language models (LLMs) struggle significantly with the fine-grained identification of these elements, underscoring the complexity of detecting hate speech. VIRC stands out as the first resource of its kind in these languages, offering a richer annotation schema compared to existing corpora. The insights derived from VIRC can inform the development of sophisticated detection tools and the creation of policies and regulations to combat hate speech on social media, promoting a safer online environment. Future work will focus on expanding the corpus and refining annotation guidelines to further enhance its comprehensiveness and reliability."
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
