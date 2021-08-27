# Utility Scoring of Product Reviews

Online shoppers generally go through other people's reviews of a specific product before actually buying it. Manufacturers can also examine product reviews to observe customer opinions and make improvements or predict market trends. Now it's undeniable that product reviews aren't equally 'useful.' 

## Objective
- In this project, we identify a task in text sentiment analysis: predicting the utility of product reviews. 
- We build regression models by incorporating various features(Subjectivity, Polarity, Flesch index, entropy, Dale Chall index, Lex diversity, Helpful Ratio, etc.) and achieving highly competitive performance for utility scoring and reviewing real-world data sets.

## Dataset
- The dataset used is obtained from [Julian McAuley's Amazon Product Reviews](http://jmcauley.ucsd.edu/data/amazon/) dataset. 
- However, due to computational limits, only a [Subset](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Cell_Phones_and_Accessories_5.json.gz) is used in this project, contains reviews for Cell Phones and Accessories category products only. 

## Result and Conclusion
- We tried out various regression models. The best two performing models were 'Gradient Boosting Regressor' and 'Random Forest Regressor,' with an R squared value of approximately 0.66 and RMSE around 0.04.

- In general, Utility Score increases with an increase in the Subjectivity Score, Polarity Score, Dale Chall Index, Helpful Ratio and decreases with an increase in Flesch Index and Entropy Score.

- Helpful Ratio came out to be the most crucial feature. It is intuitive also as a person who generally has written helpful reviews(given the advancement in the E-Commerce most of the users have some history) in the past will continue to do so. 

## References
- The project's basis is a research paper titled 'Utility Scoring of Product Reviews' by Zhu Zhang and Balaji Varadarajan. 
- Taking the inspiration from the past work, we have incorporated a few more features such as 'helpful ratio' and tried out better available regression models. 
- You can check 'References' for analysis of the past work.

## Markdown Tree

```bash
.
├── Code
│   ├── 01-Data Analysis
│   │   ├── 01.01-data_filteration.ipynb
│   │   ├── 01.02-data_conversion.ipynb
│   │   ├── 01.03-data_visualisation.ipynb
│   │   └── 01.04-data_preProcessing.ipynb
│   ├── 02-Generate Semantic Scores
│   │   ├── 02.01-generate_subjectivity_score.ipynb
│   │   ├── 02.02-generate_flesch_index.ipynb
│   │   ├── 02.03-generate_polarity_score.ipynb
│   │   ├── 02.04-generate_entropy_score.ipynb
│   │   ├── 02.05-generate_daleChall_index.ipynb
│   │   ├── 02.06-generate_helpful_ratio.ipynb
│   │   └── 02.07-generate_lexDiversity_ratio.ipynb
│   ├── 03-Normalize Semantic Scores
│   │   ├── 03.01-normalize_subjectivity_score.ipynb
│   │   ├── 03.02-normalize_flesch_index.ipynb
│   │   ├── 03.03-normalize_polarity_score.ipynb
│   │   ├── 03.04-normalize_entropy_score.ipynb
│   │   ├── 03.05-normalize_daleChall_index.ipynb
│   │   ├── 03.06-normalize_helpful_ratio.ipynb
│   │   └── 03.07-normalize_lexicalDiversity_ratio.ipynb
│   ├── 04-Visualize Semantic Scores
│   │   ├── 06.01-visualize_subjectivity_score.ipynb
│   │   ├── 06.02-visualize_flesch_index.ipynb
│   │   ├── 06.03-visualize_polarity_score.ipynb
│   │   ├── 06.04-visualize_entropy_score.ipynb
│   │   ├── 06.05-visualize_daleChall_index.ipynb
│   │   ├── 06.06-visualize_helpful_ratio.ipynb
│   │   └── 06.07-visualize_lexDiversity_ratio.ipynb
│   ├── 05-Add Target Variable
│   │   └── 05.01-add_utilityScore.ipynb
│   ├── 06-Select Models
│   │   ├── 06.01-comparing_models.ipynb
│   │   └── 06.02-tuning_selectedModels.ipynb
│   ├── 07-Final Models
│   │   ├── 07.01-gradientBoosting_regressor.ipynb
│   │   └── 07.02-randomForest_regressor.ipynb
│   └── 08-Visualize Utility Score
│       ├── 08.01-visualize_gradientBoosting.ipynb
│       └── 08.02-visualize_randomForest.ipynb
├── Data
│   ├── Cell_Phones_and_Accessories.csv
│   └── EasyWords.txt
├── README.md
└── Reference
    ├── Extended Abstract.pdf
    └── Presentation.pdf
```

