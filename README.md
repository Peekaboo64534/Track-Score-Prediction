# Track Score Prediction

## Project Overview

This project aims to predict the popularity of music tracks(Track Score) using a dataset of the most streamed Spotify songs in 2024, obtained from Kaggle. The models implemented include Linear Regression, Random Forest, Gradient Boosting, and XGBoost. The goal is to identify key features that contribute to a track's success and evaluate the performance of different models in predicting track scores.

## Dataset

### Source

The dataset used in this project is sourced from Kaggle: [Most Streamed Spotify Songs 2024](https://www.kaggle.com/datasets/nelgiriyewithana/most-streamed-spotify-songs-2024/data).

### Features

The dataset includes the following features:

- **Track Name**: The name of the song.
- **Artist Name**: The name of the artist.
- **Spotify Streams**: The number of times the track has been streamed on Spotify.
- **YouTube Views**: The number of views on YouTube for the track.
- **YouTube Likes**: The number of likes on YouTube for the track.
- **TikTok Views**: The number of views on TikTok for the track.
- **TikTok Likes**: The number of likes on TikTok for the track.
- **Shazam Counts**: The number of times the track has been identified using Shazam.
- **Playlist Counts**: The number of playlists (across Apple Music, Deezer, and Amazon) the track appears in.
- **Explicit Track**: Indicator if the track contains explicit content.
- **Release Year and Month**: The release date information.

## Methodology

### Data Preprocessing

1. **Data Cleaning**:
   - Removed missing values and handled outliers to ensure data integrity.
   - Converted categorical features to numerical using one-hot encoding for analysis.

2. **Feature Scaling**:
   - Applied scaling to numerical features using StandardScaler to standardize data and improve model performance.

3. **Feature Engineering**:
   - Created new features or transformed existing ones to enhance the model input, such as calculating engagement metrics.

### Model Selection and Training

1. **Linear Regression**:
   - Used as a baseline model to predict track scores and assess linear relationships.

2. **Decision Tree and Random Forest**:
   - Implemented to capture non-linear relationships and understand feature importance through tree-based models.

3. **Gradient Boosting**:
   - Utilized for its ability to handle complex patterns and improve prediction accuracy using ensemble learning.

4. **XGBoost**:
   - Chosen for its efficiency and performance in handling large datasets with gradient boosting techniques.

### Model Evaluation

- Evaluated models using metrics such as Mean Absolute Error (MAE) and Root Mean Square Error (RMSE).
- Conducted cross-validation to ensure model stability and reliability, checking for overfitting and underfitting.

## Results

### Feature Importance

- Analyzed feature importance scores from ensemble models (Random Forest, XGBoost) to identify the most influential features.
- **Key Features**:
  - **YouTube Views**: Strong indicator of track popularity due to broad reach and visibility.
  - **Spotify Streams**: Direct metric reflecting a track's popularity and audience engagement.
  - **TikTok Views**: Captures viral trends and youth engagement.
  - **Playlist Counts**: Influence from playlist inclusions on multiple streaming platforms drives visibility.

### Model Comparison

- Compared model performance based on MAE and RMSE metrics across various models.
- **Best Performing Model**: Random Forest demonstrated the best balance between accuracy and interpretability for this dataset.
- **Accuracy Insights**: Certain tracks with high social media engagement were predicted more accurately due to their strong feature correlations.

## Conclusion

This project highlights the potential of machine learning models in predicting music track success. By analyzing feature importance and comparing model performance, we gain valuable insights into the factors contributing to a track's popularity.

## Future Work

- Explore additional features such as artist collaborations and genres for deeper insights.
- Implement hyperparameter tuning to further optimize model performance using tools like GridSearchCV.
- Investigate model deployment for real-time predictions in streaming services.

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required libraries (see `requirements.txt`)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Peekaboo64534/Track-Score-Prediction.git

