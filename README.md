# screen_gestures_author_classification
This is upgraded version code for my Master Thesis
(https://drive.google.com/file/d/1TqnB2m4mjir9zcGYWwzK8PXVIojTvPws/view?usp=sharing)

Paper analyzes the problem of classification of patterns drawn with a stylus on the screen of the device and their authors. Machine learning methods were used for this purpose. $ 1 Unistroke (Wobbrock, Wilson, & Li, 2007) with a total of 5280 records was used. The collection contains 16 gestures performed by 11 people ten times at three different speeds (fast, moderate and slow). Each of the patterns was made 330 times in total, while one person drew 30 individual patterns. The gestures were processed into a one-dimensional signal in the preprocessing stage. The data set was randomly divided into training and test sets. 70% of the records (3696) were in the test set and 30% (1584) in the test set. For the classification of individual gestures, 21 classifiers from the sklearn library were used. The F1 measure of MLPClassifier and SVC was 1.00, while 12 classifiers exceeded the threshold F1 = 0.99. In order to classify individual authors, 16 collections containing individual gestures by 11 people were created. Each of the collections contained 330 records authored by 11 people. Therefore, the classification was made on a significantly smaller amount of data. In order to improve the classification accuracy, the number of records in the training set has been increased by changing the proportion to 80/20. 80% of the records (264) were in the training set, and 20% (66) in the test set. Depending on the type of gesture, the F1 measure of the most accurate classifier ranged from 0.63 to 0.95. The most effective and least effectively classified gestures and symmetrical gestures in relation to each other were compared. The performance of the optimized LogisticRegresion and RigdeClassifier models was compared with the LogisticRegresionCV and RigdeClassifierCV classifiers with built-in hyperparameter optimization. In order to select one of the most universal classifiers, it was decided to perform a statistical analysis of individual classifiers. The results of the classification for individual families of classifiers were compared. Linear classifiers, based on neural networks and SVC, are best suited to classify the discussed data.Two metrics for finding similarities in the classification of individual classes of multiclass sets were also proposed.
