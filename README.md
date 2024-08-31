# ERP_11358080
# Ingredient Substitution using Text and Knowledge Graph Embeddings
This repository contains the code and additional materials for the MSc Data Science project titled "Ingredient Substitution using Text and Knowledge Graph Embeddings". The project aims to develop a scalable and efficient model for ingredient substitution by leveraging a hybrid approach combining text-based language models (Word2Vec, BERT) and Knowledge Graph models (Node2Vec, GraphSAGE, GCN). The objective is to create contextually aware substitutions tailored to individual recipes.
## Introduction
The project addresses ingredient substitution in recipes by integrating both text-based and graph-based approaches to generate substitutes. The goal is to improve model scalability and accuracy in ingredient substitution using a unique combination of NLP and knowledge graph techniques.
## Repository Structure
* _Datasets_: Contains datasets like nodes_191120.csv and edges_191120.csv.

* _Pre-Processing Notebooks_: (1_X to 3_X)

* _Baseline Notebooks_: (4_X, 5_X, and 7_X)

* _Graph Creation Notebook_: (6_X)

* _Experiment Notebooks_: (8_X to 11_X)

* _Recipe1M Raw and Processed Datasets_: Contains layer1.json and processed versions (NOT STORED HERE CURRENTLY BUT CAN BE ACCESED VIA THIS - [LINK](https://drive.google.com/drive/folders/1SmoTRuAnTTXNf5dSNBXfRMk0dRc7mOnn))

## Running the Notebooks
## Prerequisites
* _Platform Setup_: The project was fully developed on Google Colab Pro, utilizing cloud-based computational resources. All experiments were conducted using Python 3 with a CPU runtime, except for the notebooks involving BERT, where a T4 GPU was employed. In both scenarios, the High RAM setting was enabled, providing access to up to 51GB of RAM.

* _Storage Check_: Minimum 6.5 GB of storage is required for data and outputs.

* _Package Installation_: 
Install the necessary packages as listed in requirements.txt using command pip install -r requirements.txt

  or 

  run the following command in the notebook before running the cells :
  
```bash
!pip install pandas nltk numpy scikit-learn networkx gensim jellyfish transformers torch torch-geometric node2
```
## Data Pre-Processing: Run notebooks in the following order:

- `1_Recipe1M_PreProcess.ipynb`

- `2_Recipe1M_Ingredient_Match.ipynb`

- `3_Validation_Set_Recipe1mSubstitution.ipynb`

- `6_KG_Creation.ipynb`

## Baseline Models and Experiments
Baselines and Experiments: Once pre-processing is done, baselines and experiments can be run independently. Notebooks are self-contained and can be executed sequentially.
## Baselines:
_Statistical Baselines_: `4_Statistical_Baselines.ipynb`

_Text-Based Baselines_: `5_Text_Based_FOOD2VEC_Ingredients_Baseline.ipynb`, `5_Text_Based_BERT_Ingredients_Baseline.ipynb`

_Knowledge Graph-Based Baselines_: `7_Graph_Based_Node2Vec_Baseline.ipynb`, `7_Graph_Based_GCN_Baseline.ipynb`

## Experiments:
- `8_Experiment1.ipynb` : Hybrid Model with BERT and GCN Embeddings

- `8_Experiment2.ipynb` : Hybrid Model with Word2Vec and Node2Vec Embeddings

-  `9_Experiment3.ipynb` : Switching to Instructions and Context-Aware Ingredients

-  `9_Experiment4.ipynb` : Revisiting Word2Vec and Node2Vec for Instructions Feature

-  `9_Experiment5.ipynb` : Exploring Attention-Based Embeddings with Batch Normalisation for Instructions Feature

-  `9_Experiment6_V1.ipynb` : Re-adopting Original Structure with Extended Training and Parallelization for Instructions Feature

-  `9_Experiment6_V2.ipynb` : Re-adopting Original Structure with Extended Training and Parallelization for Instructions Feature

-  `9_Experiment7.ipynb` : Cross-Validation for Instructions Feature

-  `9_Experiment8.ipynb` : Incorporation of Negative Sampling with contrastive loss

-  `10_Experiment9_V1.ipynb` : Neural Network Enhancement with Attention Mechanism

-  `10_Experiment9_V2.ipynb` : Neural Network Enhancement with Attention Mechanism

-  `11_Recipe_Substitute.ipynb` : Incorporating RecipeID for Qualitative Analysis
 
