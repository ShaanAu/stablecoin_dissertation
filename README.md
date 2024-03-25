# Stablecoin Anomaly Detection

This project aims to detect anomalies in stablecoin transactions using machine learning techniques. It involves a comprehensive workflow from data wrangling, preprocessing, exploratory data analysis (EDA), to model training and evaluation. The primary focus is on implementing OneClass SVM and Isolation Forest models to identify unusual patterns that deviate from the norm in stablecoin transactions.

## Project Structure

- **Data Wrangling**: Data is collected from a stablecoin statistics API, covering several stablecoins over a specified date range. The data is then aggregated and structured for analysis.
- **Data Preprocessing**: Involves handling missing values, extracting nested data, converting data types, and normalizing the data for efficient model training.
- **Exploratory Data Analysis (EDA)**: Conducted to understand the distribution, trends, and correlations within the data. This includes plotting volume over time and analyzing price movements.
- **Feature Engineering**: New features are created using moving averages, volatility indices, and normalization to enhance model performance.
- **Model Training and Evaluation**:
  - **OneClass SVM**: Tuned and evaluated using F1-score as the primary metric. The best model is selected based on the highest F1-score for anomaly detection.
  - **Isolation Forest**: An ensemble method used for anomaly detection. It is evaluated using precision, recall, and F1-score, with hyperparameters optimized through GridSearchCV.

## Key Findings

- **OneClass SVM** and **Isolation Forest** models were able to detect anomalies to varying degrees of success. The models were primarily evaluated using the F1-score, precision, recall, and ROC curves.
- EDA revealed certain trends and patterns in the stablecoin data, which were crucial for feature engineering and model training phases.
- The feature engineering step significantly improved model performance by incorporating historical and statistical insights into the dataset.

## Visualization

- Confusion matrices and ROC curves were used to visualize the performance of the models.
- Precision-Recall curves provided insights into the trade-off between precision and recall for the anomaly detection tasks.

## Challenges and Future Work

- Dealing with imbalanced data was a significant challenge, as anomalies are inherently rare in the dataset.
- Future work could explore more advanced techniques for imbalance handling, feature selection, and the integration of additional data sources to improve model robustness and accuracy.

### Running the Notebook

1. **Clone the project repository to your local machine or download the `Stablecoin Dissertation.ipynb` Jupyter Notebook directly.**

2. **Navigate to the directory containing the downloaded notebook.**

3. **Open a terminal or command prompt and run the following command to start Jupyter Notebook or JupyterLab:**

   - For **Jupyter Notebook**:
     ```bash
     jupyter notebook
     ```
   - For **JupyterLab**:
     ```bash
     jupyter lab
     ```

4. **Jupyter will open in your web browser. Navigate to `Stablecoin Dissertation.ipynb` and open it.**

5. **Run the cells in sequence from the top of the notebook to the bottom. Ensure each cell completes before moving on to the next.**

Following these steps will enable you to run the notebook and explore the anomaly detection analysis performed on stablecoin transactions.

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.8 or newer
- Jupyter Notebook or JupyterLab
- Required Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, and `requests`

You can install the required Python libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn requests
