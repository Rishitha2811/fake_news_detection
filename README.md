## Fake News Detection

* **Introduction**
    * This project is intended to built machine learning models, which will learn the patterns in the fake and non-fake text data, which can be deployed further in the real world applications.
* **Importing Modules**
    * We have used multiple python third party libraries in this project and they are:
        * re - For text preprocessing
        * glob, zipfile - modules, which deals with the files and folders
        * nltk - Used for removing stopwords and stemming
        * numpy - To make all the numerical operations faster
        * pandas - For DataFrame Munging
        * seaborn, matplotlib - Visualizing the confusion matrices
        * wordcloud - To create Wordclouds
        * Scikit Learn - This contains all the used machine learning models.
* **Data Loading**
    * The data which we have used in this project is available in the kaggle, which can be downloaded using the kaggle API
    * First, you need to install the kaggle CLI command
    * Once, it is Installed, you need to place your kaggle API key in the corresponding folder, where the kaggle command can find it to authenticate your account.
    * After everything is setup, use this command `kaggle datasets download -d sumanthvrao/fakenewsdataset` to download the dataset
* **Data Preprocessing**
    * Some of the data files contains multiple lines and punctuation marks, so we had to some preprocessing like tokenizing, merging all the words, removal of puncuation marks.
    * The next is to remove irrelavant words, which are known as stop words in the Natural Language domain.
    * Final step is to reduce all the words to their root forms, which is called stemming.
* **Data Transformation**
    * Now, the data is clean, but still we cannot feed it to the machine learning model, as they can only understand numerical datatypes, so we need to convert it to the numerical format.
    * To do that we use two methods,
        * Count vectors which are also known as the Bag of Words(BOW), where we store the frequency of each word in a sentence, in a vector format.
        * TF-IDF - Term Frequency Inverse Document Frequency, which is a extended version of the previous one.
* **Modelling**
    * We have used three different types of models
        * Logistic Regression - A simple linear model, which we have used as a baseline model, this model assumes a linear relationship between features and labels.
        * Random Forest - A ensemble of weak models, which combines the predictions of multiple models.
        * Support Vector Machines - An another non-linear model, which models a relationship between the features and labels by projecting the features into higher dimensional space.
* **Evaluation**
    * We have used two metrics, in evaluating the model preformance
        * Accuracy Score, which the percentage of matching between the actuals and predictions.
        * Confusion Matrix

* **Conclusion**
    * We have built three models, which are able to predict the fake news with an accuracy of 90%.
    * The best model is the Random Forest, which has an accuracy of 95%.
    * We can further improve the model by using the deep learning models, which are able to learn the complex patterns in the data.
    * We can also use the BERT, which is a transformer model, which is able to learn the context of the words.
    * We can also use the ensemble of models, which are able to combine the predictions of multiple models.
    * We can also use the hyperparameter tuning, which is able to find the best parameters for the model.
    * We can also use the cross validation, which is able to find the best model, which is able to generalize well on the unseen data.
    * We can also use the data augmentation, which is able to generate more data from the existing data.
    * We can also use the transfer learning, which is able to transfer the knowledge from one model to another model.
    * We can also use the active learning, which is able to learn the patterns in the data, which are hard to learn.
    * We can also use the semi-supervised learning, which is able to learn the patterns in the data, which are partially labeled.
