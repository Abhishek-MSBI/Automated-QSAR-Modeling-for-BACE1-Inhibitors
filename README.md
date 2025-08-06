🧬 Automated QSAR Modeling for BACE1 Inhibitors
End-to-end QSAR pipeline for predicting bioactivity of BACE1 inhibitors using machine learning and deep learning approaches.
Fully automated — from data acquisition to final report generation.
Ideal for computational drug discovery and M.Sc. Bioinformatics major projects..

📌 Project Overview
This project implements a fully automated Quantitative Structure–Activity Relationship (QSAR) analysis pipeline to predict the inhibitory activity (pIC₅₀) of small molecules targeting BACE1 (Beta-secretase 1) — a key enzyme in Alzheimer's disease pathology.

Here is the link : https://colab.research.google.com/drive/1UsMlJOSO7KP0rO_BpesJP-WW2tPsl0P6?usp=sharing

Designed to be modular, reproducible, and extensible, the pipeline fetches real-time data from ChEMBL, calculates molecular descriptors, trains several machine learning and deep learning models, visualizes results, and compiles everything into a professional PDF report.

🚀 Key Features
🔄 1. Dynamic Data Fetching
Downloads the latest BACE1 inhibitors and their IC₅₀ data directly from ChEMBL.

🧹 2. Robust Preprocessing
Cleans data: removes missing values, duplicates, and invalid measurements (infinity, NaNs).

Converts IC₅₀ to pIC₅₀ for better numerical modeling.

🧪 3. Descriptor Calculation
Uses RDKit to compute a comprehensive set of 2D molecular descriptors.

Designed to easily extend with other descriptor types (e.g., fingerprints, 3D).

🤖 4. Machine Learning Models
Trains and compares the following regression models:

✅ Random Forest Regressor

✅ Gradient Boosting Regressor

✅ Support Vector Regressor (SVR)

✅ Linear Regression

✅ Deep Learning Model (Keras MLP)

Performance is evaluated using:

R² Score

RMSE (Root Mean Square Error)

📊 5. Visualization
Generates high-quality plots:

Actual vs. Predicted

Residuals vs. Predicted

Feature Importance (for tree-based models)

Training loss/validation loss for Deep Learning

📄 6. Automated PDF Report
Generates a complete QSAR_Analysis_Report.pdf summarizing:

Preprocessing steps

Model results

Diagnostic plots

Performance comparison table

🛠️ Getting Started
1. Prerequisites
Ensure you have Python 3.7+ installed.

2. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/qsar-bace1.git
cd qsar-bace1
3. Create & Activate a Virtual Environment
bash
Copy
Edit
# Create virtual environment
python -m venv venv

# Activate it
# Windows
venv\Scripts\activate

# macOS/Linux
source venv/bin/activate
4. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
5. Run the QSAR Pipeline
bash
Copy
Edit
python qsar_analysis.py
📁 Output
After the script finishes execution, you'll find:

File	Description
QSAR_Analysis_Report.pdf	Final report with all metrics, tables, and visualizations
*.png	Individual plots used in the report (e.g., actual vs. predicted)
processed_data.csv (optional)	Cleaned data with descriptors and pIC₅₀ values

🔮 Planned Extensions
The project is designed to be extensible and can be upgraded with:

✅ Deep Learning models (already integrated — Keras MLP)

🔬 Molecule generation using generative models (e.g., RNNs, VAEs)

🧬 Molecular docking or ADME prediction

🌐 Web or Streamlit GUI interface

📦 Packaging as a PyPI module or CLI tool

👨‍🔬 Use Case
Ideal for:

Research projects in computational drug discovery

Bioinformatics/cheminformatics assignments

Major M.Sc. / B.Tech projects involving ML & bioactivity prediction

📚 Citation & Acknowledgment
If you use this code or approach in your academic work, please cite:

ChEMBL database

RDKit library

scikit-learn, TensorFlow

📞 Contact
Created by [Your Name] | MSc Bioinformatics
Feel free to reach out for collaboration or queries.
