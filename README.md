# Sentiment Analysis on Amazon Product Reviews

## Project Overview
This project involves sentiment analysis on Amazon product reviews, where reviews are classified as positive or negative. We use different machine learning models (Naive Bayes, Logistic Regression, SVM, and Random Forest) to classify reviews based on the text data, with an emphasis on improving model performance through feature engineering and hyperparameter tuning.

## Dataset
The dataset used is `amazon_cells_labelled.txt` from Kaggle, containing labeled Amazon product reviews:
- **review**: The text of the product review.
- **label**: The sentiment label (1 for positive, 0 for negative).

## Tools & Technologies
- **Python**: Main programming language for data processing and model implementation.
- **Pandas**: Data manipulation and analysis.
- **NLTK**: Natural language processing for text tokenization and preprocessing.
- **Scikit-learn**: Machine learning and evaluation tools.
- **Matplotlib** and **Seaborn**: For visualizations.

## Project Steps
1. **Data Loading**: Load the dataset into a Pandas DataFrame.
2. **Preprocessing**: Clean and preprocess the text data (remove special characters, tokenization, stopword removal, and lemmatization).
3. **Feature Engineering**: Vectorize text data using CountVectorizer and TF-IDF.
4. **Model Training**: Train models (Naive Bayes, Logistic Regression, SVM, Random Forest) on the training data.
5. **Model Evaluation**: Evaluate the models using accuracy, confusion matrix, ROC-AUC, and cross-validation.

## Key Insights
- **Accuracy**: The Logistic Regression model achieved the best performance with an accuracy of 75.5%.
- **Model Comparison**: Logistic Regression outperformed other models (SVM: 77.5%, Random Forest: 73.5%).
- **ROC-AUC**: The ROC-AUC score of 0.758 indicates that the model has a good ability to discriminate between positive and negative reviews.
- **Cross-Validation**: Cross-validation scores showed variability across different splits, with a mean of ~76% accuracy, indicating the model's robustness.

## Model Improvement Strategies
- **Feature Engineering**: Implemented TF-IDF vectorization and considered using n-grams for capturing more context in the reviews.
- **Advanced Models**: Evaluated other models like Logistic Regression, SVM, and Random Forest for better accuracy.
- **Hyperparameter Tuning**: Tuned models using GridSearchCV to find optimal parameters (e.g., `C=10` for Logistic Regression).
- **Cross-Validation**: Conducted k-fold cross-validation to evaluate model performance across different data splits.

## How to Run
1. Clone this repository.
2. Open the `Sentiment_Analysis.ipynb` file in Google Colab or any Jupyter environment.
3. Run the notebook to perform sentiment analysis on the Amazon product reviews dataset.

## Outcomes
- **Accurate Model**: Achieved a final model with an ROC-AUC score of 0.758 and cross-validation accuracy around 76%.
- **Insights**: The project demonstrates text preprocessing, feature engineering, and machine learning classification techniques. The use of cross-validation and model tuning provided robust performance.

## License
This project is open-source and available under the MIT License.

