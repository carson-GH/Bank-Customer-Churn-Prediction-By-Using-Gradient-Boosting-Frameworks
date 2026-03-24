# Bank-Customer-Churn-Prediction-By-Using-Gradient-Boosting-Frameworks

## Project Overview
This repository contains the complete code for our end-to-end machine learning project. We analyzed the Kaggle Playground S4E1 dataset to predict bank customer churn. Our final deliverable includes a comprehensive EDA, the training of four distinct models, and an interactive web application powered by our best-performing LightGBM model (AUC-ROC: 0.889).

## Repository Structure
- `train.csv`: The primary dataset sourced from Kaggle.
- `CDS524_Group_Project.ipynb`: The main Jupyter/Colab notebook containing our complete workflow: EDA, data preprocessing, feature engineering, model training, and performance evaluation.
- `CDS524_APP.ipynb`: A standalone notebook containing the **Gradio** code used to launch our interactive prediction UI.
- `lightgbm_churn_model.pkl`: The serialized, pre-trained optimal LightGBM model.
- `standard_scaler.pkl`: The fitted scaler used to normalize numerical features.
- `expected_columns.pkl`: The structural template to ensure consistent One-Hot Encoding during live predictions.
- `CDS524_Report.pdf`: Our comprehensive academic final report.
- `CDS524 Group Project Requirements`: The original assignment guidelines.

## How to Run the Interactive App

We have built a fully functional web interface using Gradio to demonstrate our model's real-world predictive capability. To ensure maximum reproducibility, we recommend running our demo directly via Google Colab.

### Execution Steps
1. **Open the App Script:** Open the `CDS524_APP.ipynb` file in Google Colab.
2. **Upload Required Assets:** In the left sidebar of your Colab environment, upload the following three `.pkl` files to the current directory:
   - `lightgbm_churn_model.pkl`
   - `standard_scaler.pkl`
   - `expected_columns.pkl`
3. **Install Dependencies:** The first cell in the notebook will run `!pip install gradio`. Please execute it.
4. **Launch the UI:** Run the final cell containing the Gradio script. The output will automatically generate a **Public URL** (e.g., `https://xxxx.gradio.live`).
