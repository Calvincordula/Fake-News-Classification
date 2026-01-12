# Fake News Detection: A Linguistically Informed Categorization Framework

# Project Overview
This repository contains a custom classifier designed to detect misinformation by identifying linguistic cues typical of fraudulent news articles.


# Methodology
I employed a hybrid approach combining traditional statistical methods with modern linguistic analysis:

- **Preprocessing**: Implemented tokenization, normalization, and stop word removal.
- **Vectorization**: Utilized advanced Text Vectorization and Feature Engineering.
- **Modeling**: Developed classifiers using Logistic Regression, Linear SVM and Naive Bayes.
- **Discovery**: Used LDA (Topic Modeling) to uncover "concealed topics" within the dataset.


# Key Results
- Achieved high precision in identifying fraudulent content through nuanced linguistic feature extraction.
- Demonstrated that topic-modeling-based features significantly improve classification accuracy compared to simple word-count models.

# Installation & Setup
To replicate the environment and run the notebooks, follow these steps:

1. Create and Activate the Conda Environment:

Bash

conda create --name nlp_env python=3.11 -y

conda activate nlp_env


2. Install Dependencies:

Bash

pip install -r requirements.txt


3. Download Necessary NLP Models: The project utilizes the en_core_web_sm model for Spacy:

Bash

python -m spacy download en_core_web_sm


4. Register the Environment as a Jupyter Kernel:

Bash

python -m ipykernel install --user --name=nlp_env --display-name "Python 3.11 (nlp_env)"
