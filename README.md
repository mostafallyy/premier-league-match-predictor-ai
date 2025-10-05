This project uses machine learning to predict the outcomes of English Premier League (EPL) football matches.
It leverages historical match data and team performance statistics to forecast whether a team will win or not win a given match.

By encoding match attributes such as venue, opponent, and match timing — and by applying rolling averages to performance metrics — the model captures short-term form and overall team behavior.

🧩 Key Features

Data preprocessing and cleaning of EPL match records (≈1,400 matches).

Feature engineering using:

Venue encoding (home/away)

Opponent encoding

Time & weekday extraction

Rolling averages for goals, shots, and distances

Machine Learning model:

Random Forest Classifier trained with 50 estimators and a minimum sample split of 10.

Model evaluation using:

Accuracy: ~61.2%

Precision: ~62.5% after applying rolling averages

Visual & tabular comparison of actual vs. predicted results.

🧰 Tech Stack
Category	Tools / Libraries
Data Handling	pandas, numpy
Machine Learning	scikit-learn
Environment	Google Colab, Python 3
Visualization	matplotlib, seaborn (optional)
🧪 Dataset

The dataset (matches.csv) includes historical Premier League data such as:

Match date, venue, team, opponent, and result

Goals for/against, shots, shots on target, possession, etc.

Extracted features such as hour, weekday, and encoded categories

(Note: The dataset must be placed in the same directory as the notebook.)

🚀 How to Run

Open the notebook in Google Colab
.

Upload your matches.csv dataset when prompted.

Run all cells in order to:

Preprocess and encode data

Train the Random Forest model

Evaluate and view results

You can also clone the repository locally and run:

pip install -r requirements.txt
jupyter notebook premierleagueMathcPredictioion.ipynb

📊 Results

Baseline Random Forest Model:

Accuracy: 0.6123

Precision: 0.4746

Enhanced Model (with Rolling Averages):

Precision improved to 0.625

Captures recent team form and improves prediction reliability

🔮 Next Steps

Include additional predictors (e.g., player statistics, expected goals).

Tune hyperparameters using GridSearchCV.

Add match outcome probabilities instead of binary predictions.

Visualize feature importance and prediction confidence.

👨‍💻 Author

Mostafa Ali
📅 September 2025
