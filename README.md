Mental Health Signal Detection from Reddit Using NLP and Transformers

Overview

This project investigates the application of Natural Language Processing (NLP) and transformer-based deep learning models for detecting mental health risk signals in online support group discussions. The objective was to automatically classify Reddit posts into low, medium, or high risk levels, with the long-term vision of supporting early intervention strategies in digital mental health.

The work was undertaken as part of my MSc Data Science dissertation at the University of Essex (2025).

⸻

Dataset
	•	Collected and analysed 18,000+ Reddit posts from 20 mental health–related subreddits.
	•	Applied comprehensive text preprocessing, including normalisation, URL and mention removal, tokenisation, stopword removal, and lemmatisation.
	•	Posts were labelled into risk categories using an emotion-to-risk mapping framework to support supervised learning.

⸻

Methodology
	1.	Baseline Models
	•	TF–IDF with Logistic Regression and classical machine learning algorithms for benchmarking.
	2.	Transformer-Based Models
	•	Fine-tuned DistilBERT with customised pooling mechanisms and multi-sample dropout.
	•	Applied stratified cross-validation to address class imbalance and enhance robustness.
	•	Compared performance against reference BERT and DistilBERT architectures.
	3.	Evaluation Strategy
	•	Used macro-F1, precision, recall, and confusion matrices as evaluation metrics.
	•	Conducted per-class performance analysis to assess effectiveness in minority-risk categories.

⸻

Technology Stack
	•	Languages: Python
	•	Frameworks: PyTorch, Hugging Face Transformers
	•	Libraries: scikit-learn, Pandas, NumPy, NLTK
	•	Visualisation: Matplotlib, Seaborn

⸻

Results
	•	Baseline TF–IDF models established moderate predictive performance.
	•	Transformer-based architectures substantially outperformed baselines.
	•	The customised DistilBERT with pooling and dropout achieved the highest macro-F1, demonstrating its suitability for nuanced text classification in mental health contexts.

⸻

Future Work
	•	Extend dataset to include cross-platform data (e.g., Twitter, forums).
	•	Explore real-time deployment via APIs and dashboards for continuous monitoring.
	•	Incorporate explainability methods (e.g., LIME, SHAP) to improve transparency for clinical use.
