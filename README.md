<p align="center">
    <img src="https://github.com/asc-csa/Bilingual-Text-Analysis/blob/main/2_Output/topics.PNG?raw=true" height="300">
</p>

<p align="center">
    <a href="#stars">
        <img alt="Étoiles sur GitHub | GitHub Repo stars" src="https://img.shields.io/github/stars/asc-csa/Bilingual-Text-Analysis">
    </a>
    <a href="#watchers">
        <img alt="Spectateurs sur Github | GitHub watchers" src="https://img.shields.io/github/watchers/asc-csa/Bilingual-Text-Analysis">
    </a>
    <a href="https://github.com/asc-csa/radarsat1-scripts/commits/main">
        <img alt="Dernier commit sur GitHub | GitHub last commit" src="https://img.shields.io/github/last-commit/asc-csa/Bilingual-Text-Analysis">
    </a>
    <a href="https://github.com/asc-csa/radarsat1-scripts/graphs/contributors">
        <img alt="Contributeurs sur GitHub | GitHub contributors" src="https://img.shields.io/github/contributors/asc-csa/Bilingual-Text-Analysis">
    </a>
    <a href="https://twitter.com/intent/follow?screen_name=csa_asc">
        <img alt="Suivre sur Twitter | Twitter Follow" src="https://img.shields.io/twitter/follow/csa_asc?style=social">
    </a>
</p>

## Scripts de traitement du langage naturel pour les textes bilingues (English follows)

Le traitement du langage naturel (NLP) est la branche de l'intelligence artificielle qui traite de l'utilisation d'ordinateurs pour extraire le sens des textes en langage humain (c'est-à-dire une langue comme l'anglais ou le français plutôt qu'un langage de programmation comme Python). 

Ces scripts ont été créés pour analyser la base de données interne de l'ASC sur les leçons apprises, mais ils ont depuis été généralisés et les données initiales ont été épurées. Ces scripts peuvent être appliqués à n'importe quel tableur qui contient une colonne avec du texte en anglais, en français ou dans les deux langues. Avec quelques modifications mineures, ils pourraient également être appliqués à toute autre langue prise en charge par la bibliothèque python gensim.  

- [1_Input/dummy_data.xlsx](1_Input/dummy_data.xlsx) Données d'entrée fictives. Ce fichier a été créé à partir des documents publics du l'ASC ([1](https://donnees-data.asc-csa.gc.ca/dataset/6a854752-14bb-41bc-86c9-1d20b59b79e1), [2](https://donnees-data.asc-csa.gc.ca/dataset/8b05da69-98c3-4cc9-8eee-ce6f5378dda9)).
- [2_Output/](2_Output) Tous les fichiers créés dans ce workflow. Les fichiers .xlsx sont créés par les scripts mentionnés dans leurs noms de fichiers. Les fichiers .html sont créés à l'étape 3. 
- [analyze_lessons_step1.ipynb](analyze_lessons_step1.ipynb) Ce cahier traduit le texte bilingue ENG/FRA et crée une nouvelle colonne avec le texte entièrement anglais, une autre avec le français, et une autre qui indique la langue du texte original. Il s'agit d'une étape de prétraitement. 
- [analyze_lessons_step2.ipynb](analyze_lessons_step2.ipynb) Ce cahier calcule le score de sentiment VADER (c'est-à-dire le degré de positivité ou de négativité du texte). 
- [analyze_lessons_step3.ipynb](analyze_lessons_step3.ipynb) Ce cahier effectue une modélisation thématique en utilisant l'allocation latente de Dirichlet (LDA). 


## Natural Language Processing Scripts for Bilingual Texts (Le français précède)

Natural language processing (NLP) is the branch of artificial intelligence that deals with using computers to extract meaning from human language texts (ie. a language like English or French rather than a programming language like Python). 

These scripts were originally created to analyze the CSA's internal lessons learned database, but they have since been generalized and the initial data has been scrubbed. These scripts can be applied to any spreadsheet that contains a column with text in English, French, or both. With a few minor changes, it could also be applied to any other languages supported by the gensim python library.  

- [1_Input/dummy_data.xlsx](1_Input/dummy_data.xlsx) Dummy input data. This file was created from public CSA documents ([1](https://donnees-data.asc-csa.gc.ca/dataset/6a854752-14bb-41bc-86c9-1d20b59b79e1),[2](https://donnees-data.asc-csa.gc.ca/dataset/8b05da69-98c3-4cc9-8eee-ce6f5378dda9)).
- [2_Output/](2_Output) All files created in this workflow. The .xlsx files are created by the scripts mentioned in their filenames. The .html files are created in step 3. 
- [analyze_lessons_step1.ipynb](analyze_lessons_step1.ipynb) This notebook translates the ENG/FRA bilingual text and creates a new column with fully English text, another with French, and another that indicates the language of the original text. This is a pre-processing step. 
- [analyze_lessons_step2.ipynb](analyze_lessons_step2.ipynb) This notebook calculates the VADER sentiment score (ie. how positive or negative the text is). 
- [analyze_lessons_step3.ipynb](analyze_lessons_step3.ipynb) This notebook conducts topic modelling using latent Dirichlet allocation (LDA). 
