# Solar-Prediction-Challange-GIKI
🌞 Solar Energy Forecasting Project

This project predicts solar PV generation (W) and load consumption (W) for solar energy systems up to 4 hours ahead in 10-minute intervals. It also calculates system efficiency (generation ÷ consumption).
The work includes data preprocessing, feature engineering, and model experimentation with LightGBM, XGBoost, and ensemble methods.

📂 Repository Structure
├── README.md                 <- Project documentation
├── Solar_Prediction_Final.ipynb   <- Main notebook with code, analysis, and results
├── report.pdf                <- Final project report (methods, results, discussion)
├── requirements.txt          <- Python dependencies


⚙️ Installation (Local Machine)
Clone the repository:
git clone https://github.com/Sair117/Solar-Prediction-Challange-GIKI.git
cd solar-forecasting
Install dependencies: pip install -r requirements.txt
Launch Jupyter Notebook: jupyter notebook
Open Solar_Prediction_Final.ipynb and run all cells.


▶️ Running on Google Colab (Recommended)

To avoid manual setup, you can run the notebook directly on Google Colab:
 -open github repo and download notebook
 -open colab and upload the notebook from your computer
 -alternatively you can choose github option on colab and use the link to accsses

Open Solar_Forecasting.ipynb and run all cells.

⚡ Colab will automatically handle dependencies, though you may need to install a few with !pip install ... at the top of the notebook (already included in the notebook).

📊 Dataset

The dataset consists of:

train_data.csv
test_data_masked.csv
systems_new.csv
sample_submission.csv

Due to size limits, only sample files may be included in /data.
Download the full dataset from the competition page and place it inside the /data directory (or mount Google Drive in Colab).


📈 Model Performance

Baseline: XGBoost + LSTM Ensemble → MAE = 2628

With weather features (pvlib) → MAE = 2415

With Optuna hyperparameter tuning → MAE = 2302

Final best: LightGBM with tuned parameters → MAE = 1282

👤 Author

Ahmad Adeel Sair
Email: ahmadsair2005@gmail.com
GitHub: Sair117
