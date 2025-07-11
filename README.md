# Men's March Madness Seed Prediction

This project uses NCAA men's basketball season statistics to predict March Madness seed placements using machine learning techniques. The goal was to understand what factors most influence team rankings and explore how statistical modeling can support decision-making in sports analytics.

## Project Summary

- Problem: Predict the March Madness tournament seed of a college basketball team based on season performance metrics.
- Approach: Feature engineering → Exploratory analysis → Model building → Evaluation.
- Tools Used: Python (Pandas, Matplotlib), Tableau (for visualizations)

## Dataset Features

The dataset included core metrics for each team’s season, including:
- 2-point and 3-point shooting percentages
- 2-point and 3-point shots allowed
- Wins above bubble
- Turnover and steal rates
- Athletic conference affiliation

### Feature Engineering

- Created a new Win Percentage column by dividing games won by games played.
- Dropped non-predictive or redundant columns: team name, games played/won, and postseason results.

## Exploratory Visualizations

We analyzed relationships between features using scatterplots, bar graphs, and correlation analysis:

- Offense vs. Defense: Found a weak negative correlation — elite teams were well-rounded, while others were skewed.
- Turnovers vs. Steals: No strong relationship; indicated that other factors drive turnovers.
- 2-Point Shooting vs. Win %: Showed a clear positive trend — efficient scorers tend to win more games.
- Conference Distribution: Highlighted disparities in team counts by athletic conference.

## Models and Results

Four classification algorithms were trained and tested to predict the seed of each team:

| Algorithm           | Accuracy Score |
|---------------------|----------------|
| Random Forest       | 83.7%          |
| Decision Tree       | 83.3%          |
| K-Nearest Neighbors | 83.1%          |
| Naive Bayes         | 72.1%          |

Random Forest performed the best in terms of accuracy.

## Files Included

- `march_madness_presentation.pdf`: Summary deck presenting key findings with graphs.

## Key Learnings

- Effective feature engineering and data cleaning are crucial to model success.
- Visualizing data early helps identify important trends that inform feature selection.
- Simple models like decision trees can still provide interpretable results.
- Turnover and steal rates don’t always correlate.


