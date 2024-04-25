# MERP: A Music dataset with Emotion Ratings and Raters' Profile information

"Music is capable of conveying many emotions. The level and type of emotion of the music perceived by a listener, however, is highly subjective. In this study, we present the Music Emotion Recognition with Profile information dataset (MERP). This database was collected through Amazon Mechanical Turk (MTurk) and features dynamical valence and arousal ratings of 54 selected full-length songs. The dataset contains music features, as well as user profile information of the annotators. The songs were selected from the Free Music Archive using an innovative method (a Triple Neural Network with the OpenSmile toolkit) to identify 50 songs with the most distinctive emotions. Specifically, the songs were chosen to fully cover the four quadrants of the valence-arousal space. Four additional songs were selected from the DEAM dataset to act as a benchmark in this study and filter out low quality ratings. A total of 452 participants participated in annotating the dataset, with 277 participants remaining after thoroughly cleaning the dataset. Their demographic information, listening preferences, and musical background were recorded. [...]"

## Key points
- Continuous valence/arousal annotations and continuous audio features available
- Large number of audio features (>260)
- Allows correlation between audio features and emotional rating
- Allows correlation analysis between music and raters' taste profile
- Read the paper as many statistical tests are already performed by the authors!

## Difficulty score
The diffculty score for this dataset is 0.75. However, if you are only using the questionnaire variables from the raters' profile information as the dependent and independent variables, then no preprocessing is required which would result in a bonus score of 0. 

For a maximum score: If you are succesfully processing and using at least two continuous audio features and the continuous valence and arousal annotations in your statistical analysis, you obtain 0.75 bonus points. Processing and feature extraction should not be trivial.


## Access

Access the dataset via [Kaggle](https://www.kaggle.com/datasets/kohenyan/music-emotion-recognition-with-profile-information?select=pinfo.pkl)

This dataset also has a Github Repository available: https://github.com/dorienh/MERP

## Paper

> Koh, E. Y., Cheuk, K. W., Heung, K. Y., Agres, K. R., & Herremans, D. (2022). MERP: a music dataset with emotion ratings and raters’ profile information. Sensors, 23(1), 382.

https://www.mdpi.com/1424-8220/23/1/382
