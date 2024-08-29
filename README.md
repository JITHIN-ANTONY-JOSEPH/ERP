# ERP_11358080
# Ingredient Substitution using Text and Knowledge Graph Embeddings
This repository contains the code and additional materials for the MSc Data Science project titled "Ingredient Substitution using Text and Knowledge Graph Embeddings". The project aims to develop a scalable and efficient model for ingredient substitution by leveraging a hybrid approach combining text-based language models (Word2Vec, BERT) and Knowledge Graph models (Node2Vec, GraphSAGE, GCN). The objective is to create contextually aware substitutions tailored to individual recipes.
### Introduction
The project addresses ingredient substitution in recipes by integrating both text-based and graph-based approaches to generate substitutes. The goal is to improve model scalability and accuracy in ingredient substitution using a unique combination of NLP and knowledge graph techniques.
### Repository Structure
Datasets: Contains datasets like nodes_191120.csv and edges_191120.csv.

Pre-Processing Notebooks: (1_X to 3_X)

Baseline Notebooks: (4_X, 5_X, and 7_X)

Graph Creation Notebook: (6_X)

Experiment Notebooks: (8_X to 11_X)

Recipe1M Raw and Processed Datasets: Contains layer1.json and processed versions (NOT STORED HERE CURRENTLY BUT CAN BE ACCESED VIA THIS - [LINK](https://drive.google.com/drive/folders/1SmoTRuAnTTXNf5dSNBXfRMk0dRc7mOnn))

## Running the Notebooks
### Prerequisites
_Platform Setup_: Google Colab or any Python environment with necessary packages.

_Storage Check_: Minimum 6.5 GB of storage is required for data and outputs.

_Package Installation_: 
Install the necessary packages as listed in requirements.txt using command pip install -r requirements.txt
or 
run the following command in the notebook before running the cells : !pip install pandas nltk numpy scikit-learn networkx gensim jellyfish transformers torch torch-geometric node2

### Data Pre-Processing: Run notebooks in the following order:
1_Recipe1M_PreProcess.ipynb

2_Recipe1M_Ingredient_Match.ipynb

3_Validation_Set_Recipe1mSubstitution.ipynb

### Baseline Models and Experiments
Baselines and Experiments: Once pre-processing is done, baselines and experiments can be run independently. Notebooks are self-contained and can be executed sequentially.
### Baselines:
_Statistical Baselines_: 4_Statistical_Baselines.ipynb

_Text-Based Baselines_: 5_Text_Based_FOOD2VEC_Ingredients_Baseline.ipynb, 5_Text_Based_BERT_Ingredients_Baseline.ipynb

_Knowledge Graph-Based Baselines_: 7_Graph_Based_Node2Vec_Baseline.ipynb, 7_Graph_Based_GCN_Baseline.ipynb

### Experiments:
Experiments are numbered from 8_Experiment1.ipynb to 11_RECIPE_SPECIFIC.ipynb and explore various model combinations and improvements.
