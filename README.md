# Group 13: News Article Recommender System

This repository hosts Group 13's project submission, a recommender system for news articles leveraging a large language model (LLM). This session-based content-driven system matches users' natural language queries to relevant news topics, while incorporating user feedback and ensuring diversity in the results.

## Repository Structure

Our repository comprises three Jupyter notebooks and two primary folders as follows:

### Jupyter Notebooks

1. **`model_generation.ipynb`**: This notebook generates the vector store essential for our minimum viable product (MVP). It identifies and embeds topics from news articles into a FAISS vector store, which is stored locally. The notebook also contains additional analysis of the extracted topics.

2. **`evaluation.ipynb`**: This notebook assembles the necessary tools for MVP evaluation. It generates 100 contextually relevant queries based on randomly selected news articles. A pipeline for evaluating recommendations when the user's query aligns with the suggested article is also established. Generated queries and developed prompt templates are stored locally.

3. **`llm_prediction.ipynb`**: This is the central notebook for building the MVP. It facilitates the search function, integration of user feedback, and a user interface for interaction with the recommender system. The notebook utilizes the vector store and developed prompts for evaluation. This is the only repository taht needs to be run if you simply want to explore the recommender system.

### Folders

1. **`Data`**: This folder contains cleaned and raw DataFrames, and the OpenAI key file.

2. **`prompt_templates`**: This folder houses developed prompt templates and zero-shot examples for this project. It has three subfolders, each with a different purpose:

    - **`evals`**: Prompts ussed for evaluation of the recommender system. 
    - **`generate`**: Prompts and Examples used in the building of the vector store.
    - **`recommendations`**: Prompts used in the recommendation prototype.
    
3. **`Figures`**: This folder contains figures created for the report and better understanding.

4.  **`Results`**: This folder contains the obtained results from the evaluation pipeline. The data is stored in json and the filename should explain what it represents/the settings of the evaluation.


# NewsRecommenderLLM
