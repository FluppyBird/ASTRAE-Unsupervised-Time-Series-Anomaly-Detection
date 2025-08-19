# ASTRAE – Unsupervised Time Series Anomaly Detection

## 📂 Repository Structure

| Path | Description |
|------|-------------|
| `Autoencoder_for_Anomaly_detection.ipynb` | Main notebook for training the Autoencoder model for anomaly detection. |
| `data_analytics_preprocessing.ipynb` | Notebook for performing initial data cleaning and preprocessing. |
| `Anomaly_figures/` | Folder containing visualization results generated after running the notebooks (e.g., anomaly score plots, detected anomaly timestamps, etc.). |
| `train_val_mse_loss/` | Folder containing figures of the model’s training and validation MSE loss curves. |
| `dataset/` | Folder with the input time series datasets used in the experiments. |
| `loss_history_LSTM_baseline.xlsx` | Loss history of a baseline LSTM model (for comparison purposes). |
| `loss_history_dense.xlsx` | Loss history of a baseline dense network (for comparison purposes). |
| `root directory.png` | Overview diagram showing the overall project structure. |

## 🧱 Project Overview

The project uses **unsupervised learning techniques (Autoencoder and baseline LSTM)** to learn the normal patterns of the input time series. Anomalies are detected based on the **reconstruction error** produced by the trained model.

The workflow includes:
1. **Data Preprocessing** – Performed in `data_analytics_preprocessing.ipynb`, including normalization and sequence generation.
2. **Model Training** – Conducted in `Autoencoder_for_Anomaly_detection.ipynb`.
3. **Evaluation & Visualization** – After training, anomaly scores and loss curves are visualized.  
   - Output figures are stored in the `Anomaly_figures` and `train_val_mse_loss` folders.

> 📌 **Note**: The `.ipynb` files contain the code necessary to reproduce the training and evaluation. To reproduce the results, simply run the notebooks in order (preprocessing → training).

## ✅ How to Run

1. Clone the repository:
   ```
bash
git clone https://github.com/FluppyBird/ASTRAE-Unsupervised-Time-Series-Anomaly-Detection.git
cd ASTRAE-Unsupervised-Time-Series-Anomaly-Detection
   ```
2. Open the preprocessing notebook and run all cells:
   `data_analytics_preprocessing.ipynb`
3. Open the training notebook and run all cells:
   `Autoencoder_for_Anomaly_detection.ipynb`
