Gmail Spam detection using NLP 


The project begins by importing the required libraries, including pandas and numpy, to handle data processing and manipulation. It loads a dataset ('SPAM.csv') containing information about messages and their types (spam or ham) using the pandas library.

Next, the code maps the 'type' column values to binary labels, assigning 1 for spam and 0 for ham. This allows the dataset to be transformed into a format suitable for classification models.

The code performs some exploratory data analysis by displaying the column names and the number of rows in the 'type' and 'text' columns.

To prepare the text data for analysis, the code tokenizes the text by splitting it into individual words. It then applies stemming and lemmatization techniques to normalize the words, reducing them to their base or root form. Stop words, which are commonly occurring words with little semantic meaning, are removed from the text using a predefined set of stopwords.

The preprocessed text is then transformed into numerical feature vectors using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization technique. This captures the importance of each word in the text relative to the entire dataset.

The dataset is split into training and testing sets using the train_test_split function from scikit-learn. Two classifiers, Logistic Regression and Linear Support Vector Machine (SVM), are trained on the training set and evaluated on the testing set.

Finally, the models make predictions on the testing set, and their respective performance can be assessed using appropriate evaluation metrics.

Overall, this project aims to detect spam messages by leveraging machine learning algorithms and various text preprocessing techniques, ultimately providing a means to identify and filter out unwanted communication.
