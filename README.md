# EV-Pred
📂 Project Structure
The notebook (EV_Pred.ipynb) is organized into the following key stages:

Data Acquisition

Downloads battery data from NASA’s Prognostics dataset (fallback to synthetic data if download fails).

Exploratory Data Analysis (EDA)

Visualizes key trends, such as capacity degradation and charge cycles.

Identifies patterns in voltage, temperature, and current.

Data Preprocessing

Normalizes and reshapes data for sequence models.

Creates train-test splits for evaluation.

Modeling Approaches

LSTM (PyTorch): Sequence model for predicting capacity degradation.

Random Forest (Sklearn): Baseline ensemble model.

XGBoost: Gradient-boosted model for improved performance.

Model Evaluation

Evaluates each model using MAE, RMSE, and R² scores.

Visual comparison of true vs predicted values.

Conclusion

Highlights the best-performing model.

Estimates remaining useful life (RUL) for battery cells.

🛠️ Technologies Used
Python

NumPy, Pandas

Matplotlib, Seaborn

Scikit-learn

XGBoost

PyTorch (for LSTM)

NASA Battery Dataset

📊 Sample Results
LSTM showed the highest performance in predicting long-term battery health.

XGBoost offered a strong non-sequential baseline.

Visualizations reveal how each model captures degradation trends.

🚀 How to Run
Clone the repository or download the notebook.

Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the notebook: EV_Pred.ipynb using Jupyter Notebook or any compatible IDE.

Note: Internet access is required to download the NASA dataset.

📌 Future Work
Extend to real-world EV fleet data.

Add anomaly detection for early fault diagnosis.

Integrate RUL predictions into EV dashboard simulations.

📄 License
This project is for educational and research purposes. Refer to the NASA PCoE data license for dataset usage terms.
