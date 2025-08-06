Automated QSAR Modeling for BACE1 Inhibitors
This project contains a Python script that performs an end-to-end Quantitative Structure-Activity Relationship (QSAR) analysis for inhibitors of the BACE1 enzyme, a key target in Alzheimer's disease research.

The workflow automates every step of the process, from data acquisition to final reporting, making it a powerful tool for computational drug discovery.

Features
Dynamic Data Fetching: Automatically downloads the latest BACE1 bioactivity data (IC50 values) directly from the ChEMBL database.

Robust Preprocessing: Includes rigorous data cleaning steps to handle missing values, duplicates, and potential data errors (infinity, NaN).

Automated Descriptor Calculation: Uses the RDKit library to calculate a comprehensive set of 2D molecular descriptors for each compound.

Comparative Model Training: Trains and evaluates multiple common machine learning regression models to find the best performer:

Random Forest

Gradient Boosting

Support Vector Regressor (SVR)

Linear Regression

Comprehensive Visualization: Generates high-quality, detailed plots for in-depth model diagnostics:

Actual vs. Predicted plots to assess performance.

Residuals vs. Predicted plots to check for systematic errors.

Feature Importance plot for the best model to understand which molecular properties drive activity.

Automated PDF Reporting: Automatically compiles all results, tables, and plots into a single, professional QSAR_Analysis_Report.pdf for easy sharing and documentation.

How to Use
1. Prerequisites
Ensure you have Python 3.7 or newer installed.

2. Clone the Repository
git clone <your-repository-url>
cd <your-repository-name>

3. Set Up the Environment
It is highly recommended to use a virtual environment to manage dependencies.

# Create a virtual environment
python -m venv venv

# Activate the environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

4. Install Dependencies
Install all the required libraries using the requirements.txt file.

pip install -r requirements.txt

5. Run the Analysis
Execute the main script. The process will take a few minutes as it fetches data, calculates descriptors, and trains multiple models.

python qsar_analysis.py

6. View the Output
After the script finishes, you will find the following new files in your project directory:

QSAR_Analysis_Report.pdf: The final, comprehensive report with all results and plots.

Several .png image files: These are the individual plots that were embedded in the PDF.
