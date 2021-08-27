## Steps
To run the project, download and unzip the [JSON](http://snap.stanford.edu/data/amazon/productGraph/categoryFiles/reviews_Cell_Phones_and_Accessories_5.json.gz)  file and keep it and all the source codes in one folder. Sequentially navigate to different folders and run all the source codes in them. 

- [01-Data Analysis](01-Data%20Analysis): We will get a CSV file by the end of [01.02-data_conversion.ipynb](01-Data%20Analysis/01.02-data_conversion.ipynb) will be used in the following steps.
- [02-Generate Semantic Scores](02-Generate%20Semantic%20Scores): This step will generate all the semantic scores and add their column in the CSV file.
- [03-Normalize Semantic Scores](03-Normalize%20Semantic%20Scores): This step will normalize all the semantic scores and add their column in the CSV file. We can also skip this process based on the model we are using.
- [04-Visualize Semantic Scores](04-Visualize%20Semantic%20Scores):  This step is to visualize and analyze the semantic scores. We can add more visualizations according to our needs.
- [05-Add Target Variable](04-Visualize%20Semantic%20Scores): This step will calculate and add a column with a target variable for our model.
- [06-Select Models](06-Select%20Models): This step is to compare and tune different regression models. 
- [07-Final Models](07-Final%20Models): This step trains the selected models from the above step. 
- [08-Visualize Utility Score](08-Visualize%20Utility%20Score): This step is to visualize and analyze the utility score predicted by the model. You can add more visualization as per need.
- 

## Markdown Tree

```bash
.
├── 01-Data Analysis
│   ├── 01.01-data_filteration.ipynb
│   ├── 01.02-data_conversion.ipynb
│   ├── 01.03-data_visualisation.ipynb
│   └── 01.04-data_preProcessing.ipynb
├── 02-Generate Semantic Scores
│   ├── 02.01-generate_subjectivity_score.ipynb
│   ├── 02.02-generate_flesch_index.ipynb
│   ├── 02.03-generate_polarity_score.ipynb
│   ├── 02.04-generate_entropy_score.ipynb
│   ├── 02.05-generate_daleChall_index.ipynb
│   ├── 02.06-generate_helpful_ratio.ipynb
│   └── 02.07-generate_lexDiversity_ratio.ipynb
├── 03-Normalize Semantic Scores
│   ├── 03.01-normalize_subjectivity_score.ipynb
│   ├── 03.02-normalize_flesch_index.ipynb
│   ├── 03.03-normalize_polarity_score.ipynb
│   ├── 03.04-normalize_entropy_score.ipynb
│   ├── 03.05-normalize_daleChall_index.ipynb
│   ├── 03.06-normalize_helpful_ratio.ipynb
│   └── 03.07-normalize_lexicalDiversity_ratio.ipynb
├── 04-Visualize Semantic Scores
│   ├── 06.01-visualize_subjectivity_score.ipynb
│   ├── 06.02-visualize_flesch_index.ipynb
│   ├── 06.03-visualize_polarity_score.ipynb
│   ├── 06.04-visualize_entropy_score.ipynb
│   ├── 06.05-visualize_daleChall_index.ipynb
│   ├── 06.06-visualize_helpful_ratio.ipynb
│   └── 06.07-visualize_lexDiversity_ratio.ipynb
├── 05-Add Target Variable
│   └── 05.01-add_utilityScore.ipynb
├── 06-Select Models
│   ├── 06.01-comparing_models.ipynb
│   └── 06.02-tuning_selectedModels.ipynb
├── 07-Final Models
│   ├── 07.01-gradientBoosting_regressor.ipynb
│   └── 07.02-randomForest_regressor.ipynb
├── 08-Visualize Utility Score
│   ├── 08.01-visualize_gradientBoosting.ipynb
│   └── 08.02-visualize_randomForest.ipynb
└── README.md

```

