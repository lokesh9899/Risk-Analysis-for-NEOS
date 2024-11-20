# NEO Detection: Predicting Near-Earth Object Hazards

This project focuses on predicting the hazard level of Near-Earth Objects (NEOs) using machine learning models. It includes exploratory data analysis, feature engineering, and model evaluation. The insights and predictions aim to assist in identifying potentially hazardous asteroids based on their physical and orbital characteristics.

---

## Features of the Project
1. **Data Exploration**:
   - Explored distributions of NEO features like brightness, size, velocity, and miss distance.
   - Identified key patterns and correlations, such as the inverse relationship between size and brightness.

2. **Machine Learning Models**:
   - **Random Forest**: Best-performing model with high accuracy, recall, and precision.
   - **XGBoost**: Robust boosting algorithm delivering competitive results.
   - **Ensemble Models**:
     - **Voting Classifier**: Combined multiple models for a balanced prediction.
     - **Stacking Classifier**: Improved recall and precision through layered predictions.
   - Baseline Models: Logistic Regression and Decision Tree for initial comparisons.

3. **Deployment**:
   - Deployed the Random Forest model using **Gradio** for interactive hazard predictions.

---

## Insights from the Analysis
1. **Data Characteristics**:
   - Brightness and size are inversely correlated: brighter objects are typically larger.
   - Hazardous objects have smaller miss distances and occasionally higher velocities.

2. **Model Performances**:
   - **Random Forest**: Achieved a balanced performance with:
     - Accuracy: 88%
     - Precision: 91%
     - Recall: 88%
     - F1 Score: 89%
     - ROC-AUC: 0.94
   - Ensemble models further balanced precision and recall for challenging classifications.

3. **Visualization**:
   - Scatter plots, heatmaps, and histograms provided clear insights into data distribution and relationships.

4. **Deployment**:
   - The model predicts "Hazardous" or "Safe" based on six input features: absolute magnitude, size, velocity, proximity, and risk factors.

---

## Project Workflow
1. **Data Preparation**:
   - Cleaned and preprocessed data.
   - Handled missing values and encoded categorical features.

2. **Exploratory Data Analysis**:
   - Explored distributions and correlations.
   - Identified outliers and skewed distributions.

3. **Model Building**:
   - Trained multiple models with hyperparameter tuning.
   - Evaluated models using cross-validation and metrics like precision, recall, F1 score, and ROC-AUC.

4. **Deployment**:
   - Interactive Gradio application for real-time hazard prediction.

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-url.git

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost gradio

3. Run the notebook or Gradio app:
   To explore the notebook:
   ```bash
   jupyter notebook NEO_EDA_Modeling.ipynb
   
5. To launch the Gradio app:
   ```bash
   python app.py
