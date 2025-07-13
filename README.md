In this project, I am looking into the **Liar Dataset** from Kaggle to build a false statement detection model. 

## Objective 🎯
1. Classify political statements as True, Half-True, or False
2. Compare traditional models (Logistic Regression, SVM) with deep learning models (LSTM, BERT)
3. Explore the impact of metadata (speaker, party, context) on accuracy

## Dataset 📊 
1. Sourced from [Kaggle](https://www.kaggle.com/datasets/yuktibishambu/liar-dataset-labeled/data)
2. 12.8K labeled political statements from PolitiFact, each statement includes text + metadata (speaker, party, context, etc.)
3. Preprocessed into 3 categories: True, Half-True, False

## Methodology 🔧 
1. Text Preprocessing: Lowercasing, tokenization, stopword removal, stemming
2. Feature Engineering: TF-IDF, metadata features (e.g., speaker credibility)
3. Models Used:
   - Logistic Regression & SVM (with metadata + TF-IDF)
   - LSTM and BERT (text only)

## Results 📈 
Logistic Regression and SVM offered the best trade-off of precision, recall, and interpretability in this context.

## Key Insights 💡 
1. False statements were the most common, especially in healthcare topics
2. Metadata features like speaker history improved traditional model performance
3. BERT had the best recall for detecting falsehoods but low precision

## Future Work 🔮 
1. Fine-tune BERT with more epochs and metadata fusion
2. Add emotion/sentiment features
3. Build cascaded/hybrid models for explainability and accuracy

The Python notebook is available on [Kaggle](https://www.kaggle.com/code/yuktibishambu/yk-liar-data-analysis) as well as in this [repository](./yk-liar-data-analysis.ipynb). 
Read the full project report here [(PDF)](./Yukti_Sathya_project_report.pdf)
