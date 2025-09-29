# Data Science 
This repository contains two separate exercises, each implemented as a Jupyter Notebook and organized into its own folder.

## Project Structure
- `Crawling/` → Part A of the assignment (Data Collection)
- `TextClassification/` → Part B of the assignment (Machine Learning on Legal Texts)

Each folder includes:
- A Jupyter Notebook (`.ipynb`) with the full code and outputs.
- A `README.md` file explaining the approach, methodology, and results in detail.
- Exersice description

##  Exercise A: Data Collection of Supreme Court Decisions
In this part, we develop a **web crawler** to collect data from the official website of the Greek Supreme Court (Άρειος Πάγος).  
The notebook:
- Scrapes judicial decisions from the year 2024.  
- Extracts metadata such as decision number, section, judges, cited articles of law, etc.  
- Stores the data in a structured **DataFrame** (CSV).  
- Performs initial exploratory analysis with visualizations.

➡️ For more information, read the [Crawling/README.md](Crawling/README.md).

##  Exercise B: Machine Learning on Greek Legal Texts
In this part, we apply **supervised and unsupervised machine learning methods** on Greek legal documents.  
The notebook includes:
1. **Legal Document Classification**  
   - Predicts document labels (collection, chapter, topic) using models such as SVM, Logistic Regression with embeddings, and one additional classifier.  
   - Evaluated with accuracy, precision, recall, and F1-score.  

2. **Topic Modeling of Legal Decisions**  
   - Performs clustering of court decisions using K-Means and embeddings (TF-IDF or dense).  
   - Evaluates clusters with Silhouette and NMI scores.  
   - Uses a **Large Language Model (LLM)** to automatically generate descriptive titles for each cluster.

➡️ For more information, read the [TextClassification/README.md](TextClassification/README.md).

## Requirements
- Python 3.9+
- Jupyter Notebook
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `gensim`, `unsloth`, `huggingface_hub`
