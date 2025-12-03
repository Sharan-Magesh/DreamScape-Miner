# DreamScape Miner: Linking Dream Narratives to Sleep Quality

## 📌 Project Overview
**DreamScape Miner** is a multi-modal data mining project that investigates the link between qualitative dream narratives and quantitative sleep metrics. By integrating text mining (LDA Topic Modeling) with structured health data analysis, this project aims to bridge the gap between subjective dream experiences and objective sleep quality indicators.

This project was developed as part of the **CSE 572: Data Mining** course at Arizona State University.

## 📂 Dataset
The project utilizes a synthetic paired dataset derived from two open-source sources:
1.  **Sleep Health and Lifestyle Dataset:** Structured data on sleep duration, stress levels, and physical activity for 374 individuals.
2.  **Dream Symbols Dataset:** Qualitative text descriptions of dream symbols and narratives.

## 🛠️ Methodology
* **Data Integration:** Merging unstructured text with structured tabular data.
* **Natural Language Processing:** * **TF-IDF** for feature extraction.
    * **Latent Dirichlet Allocation (LDA)** for topic modeling to categorize dream themes.
* **Predictive Modeling:** * **Classifiers:** Logistic Regression, Decision Tree, and Random Forest.
    * **Target:** A "Composite Sleep Score" derived from sleep duration and quality.
* **Feature Engineering:** Removing "Stress Level" to prevent label leakage and isolating the predictive power of dream narratives.

## 🚀 Results
* **Baseline Performance:** Models achieved ~91% accuracy when including stress levels, due to high correlation.
* **True Performance:** After removing stress to isolate dream impact, the **Random Forest** model achieved **~65% accuracy**, demonstrating that dream narratives offer a modest but non-zero predictive signal for sleep quality.

## 💻 Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/DreamScape-Miner.git](https://github.com/YOUR_USERNAME/DreamScape-Miner.git)
