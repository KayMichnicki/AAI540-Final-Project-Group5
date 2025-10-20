README – Soccer Match Outcome Prediction
This project is a part of the AAI-540 course in the Applied Artificial Intelligence Program at the University of San Diego. 

-- Project Status: Completed

Installation:
1. Clone the repository:
   git clone https://github.com/KayMichnicki/AAI540-Final-Project-Group5.git
   cd AAI540-Final-Project-Group5
2. Install the required dependencies:
   pip install -r requirements.txt
3. Launch the notebook in Amazon SageMaker Studio or locally with Jupyter notebook.
4. Follow the steps in the notebook to:
   - Load and preprocess the dataset
   - Train and evaluate the models
   - Run predictions on test data

Project Intro/Objective:
The main purpose of this project is to predict the outcomes of international soccer (football) matches using historical data. Specifically, the model forecasts whether the home team wins, the away team wins, or if the match ends in a draw.

This predictive model can be applied to:
- Pre-match forecasting for analysts and fans
- Strategic decision-making for teams and organizations
- Exploratory analysis of team performance trends over time

Contributors: 
- Kay Michnicki
- Matt Thompson

Methods Used:
- Inferential Statistics
- Data Visualization
- Data Manipulation
- Machine Learning
- Cloud Computing 

Technologies:
- Python
- Amazon SageMaker
- AWS S3
- XGBoost
- pandas
- Git / GitHub
- SQL

Project Description:
We built a time-classification pipeline using 150 plus years of international soccer match data to predict match outcomes (Home Win/Draw/Away Win).
Dataset: Kaggle International Football Results
- 40,000+ matches
- Variables include team names, scores, match dates, venues, tournaments

Feature Engineering:
- ELO rating deltas
- Recent performance streaks
- Home advantage
- Head-to-head history
- Rest days

Modeling:
- Logistic Regression (baseline)
- XGBoost (final model)
- Accuracy: 61.4% | Macro-F1: 0.59

Challenges:
- Historical rule changes affecting gameplay dynamics over 150+ years
- Difficulty predicting outcomes based solely on historical team data, since player rosters, team strategies, and competition contexts change over time, and much of the retained information reflects team-level playing style or techniques rather than current performance.
- Class imbalance (fewer draws)
- Era drift in features over time

Mitigations:
- Add a rule change feature
- Use resample techniques
- Use class weight
- Features engineering
- Model tuning

License:
Graduate Programs, University of San Diego

Acknowledgments:
   • AAI-540: Machine Learning Operations, Applied Artificial Intelligence, University of San Diego
   • Professors Sean Coyne for guidance on model design and deployment
   • Amazon SageMaker Student Account for cloud infrastructure support
   • Kaggle for providing the soccer dataset
