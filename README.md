# 🧬 Automated QSAR Modeling for BACE1 Inhibitors

End-to-end QSAR pipeline for predicting the bioactivity (pIC₅₀) of BACE1 inhibitors using machine learning and deep learning in Google Colab.
Fully automated — from real-time data fetching to final PDF reporting.

## Hugging face application: [Link](https://huggingface.co/spaces/srabhishek/BACE1-QSAR-Predictor)

📌 Project Overview
This project performs Quantitative Structure–Activity Relationship (QSAR) analysis for BACE1 inhibitors, a promising target in Alzheimer's research. The entire workflow is built and executed within Google Colab, requiring no local setup or installation.

The pipeline automatically fetches bioactivity data from ChEMBL, calculates molecular descriptors, trains ML/DL models, generates visualizations, and exports a complete PDF report.

🔧 Technologies Used
Category	Libraries / Tools Used
Data Fetching	chembl_webresource_client, pandas
Descriptor Calc	RDKit
Machine Learning	scikit-learn, matplotlib, seaborn
Deep Learning	TensorFlow (Keras)
Visualization	matplotlib, seaborn
Reporting	fpdf, PIL, datetime

⚙️ How to Use (Google Colab)
✅ 1. Open the Notebook
You can directly access and run the project here:

👉 Open in Google Colab
(https://colab.research.google.com/drive/1UsMlJOSO7KP0rO_BpesJP-WW2tPsl0P6?usp=sharing)

✅ 2. Enable GPU (Optional)
Go to Runtime → Change Runtime Type

Set Hardware Accelerator to GPU (for deep learning training)

✅ 3. Run the Notebook
Click Runtime → Run All

The notebook will:

Fetch BACE1 data from ChEMBL

Clean & process it

Calculate 2D molecular descriptors

Train multiple ML models

Train a deep learning model (Keras MLP)

Generate visualizations

Save results and create QSAR_Analysis_Report.pdf

📊 Models Used
✅ Machine Learning Models
Random Forest Regressor

Gradient Boosting Regressor

Support Vector Regressor (SVR)

Linear Regression

✅ Deep Learning Model
Keras-based MLP (Multi-Layer Perceptron) with Dropout & EarlyStopping

📁 Output
File	Description
QSAR_Analysis_Report.pdf	Full report including model scores & plots
actual_vs_predicted.png	Predicted vs. true values (all models)
residuals.png	Residuals diagnostic plot
feature_importance.png	Feature importance for RF/GBM
dl_loss_plot.png	Deep Learning loss (train vs val)

🔮 Possible Extensions
You can further upgrade this project with:

🧠 Molecule generation using RNNs, VAEs, or generative models

🧪 Predicting ADME/Tox properties

📊 Integrating Streamlit or Gradio interface

🧬 3D descriptor or fingerprint-based QSAR

🗂️ Batch processing for multiple targets (multi-task QSAR)

📚 Academic Relevance
This project can be submitted as a Major Project for:

M.Sc. Bioinformatics / Biotechnology

M.Tech / B.Tech Bioinformatics

Computational drug discovery research

Includes real-world databases, ML, DL, visualization, and reporting — ideal for showcasing practical bioinformatics skills.

✍️ Author
#### Abhishek S R
#### M.Sc. Bioinformatics,
#### Garden City University

📌 Want to Use Locally?
While this project is Colab-based, you can also convert it into a standalone script:

Export notebook as .py (File → Download → .py)

Install requirements with pip install -r requirements.txt

Run via python qsar_analysis.py

If you’d like, I can help generate that .py version and requirements.txt for GitHub.
