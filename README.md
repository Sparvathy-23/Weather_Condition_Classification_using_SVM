# Weather_Condition_Classification_using_SVM

## Objective

The objective of this project is to develop a Support Vector Machine (SVM) classification model to predict whether the weather is **Warm** or **Cool** using meteorological data obtained from the Open-Meteo API. The model is trained using weather attributes such as temperature, relative humidity, surface pressure, and wind speed.

---

## API Documentation

**Open-Meteo Weather API:** https://open-meteo.com/

---

## Libraries Used

* Python
* Requests
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## Methodology

1. Retrieved historical weather data from the Open-Meteo API.
2. Converted the JSON response into a Pandas DataFrame.
3. Selected the following input features:

   * Temperature
   * Relative Humidity
   * Surface Pressure
   * Wind Speed
4. Created a target variable (`Weather_Class`):

   * Warm → Temperature ≥ 25°C
   * Cool → Temperature < 25°C
5. Checked for missing values and removed unnecessary columns.
6. Encoded the target variable using `LabelEncoder`.
7. Split the dataset into 80% training data and 20% testing data.
8. Standardized the feature values using `StandardScaler`.
9. Trained an SVM classifier with the RBF kernel.
10. Evaluated the model using Accuracy, Precision, Recall, F1-Score, Classification Report, and Confusion Matrix.

---

## Results

The Support Vector Machine classifier successfully classified weather conditions into Warm and Cool categories using the selected meteorological features. After preprocessing and feature scaling, the model achieved reliable classification performance. The evaluation metrics indicated that the classifier was able to distinguish between the two weather classes effectively, and the confusion matrix showed that most observations were correctly classified.

---

## Observations

1. The SVM classifier achieved good classification performance, indicating that weather parameters such as temperature, humidity, pressure, and wind speed are effective predictors of weather conditions.

2. Feature scaling using `StandardScaler` significantly improved the performance of the SVM model because SVM is sensitive to differences in feature magnitudes.

3. The confusion matrix showed that the majority of weather samples were classified correctly, resulting in high accuracy and balanced precision, recall, and F1-score.

---

## Conclusion

This project successfully developed a Support Vector Machine (SVM) classifier to classify weather conditions as Warm or Cool using data collected from the Open-Meteo API. The preprocessing steps, including data cleaning, label encoding, train-test splitting, and feature scaling, prepared the dataset for effective model training. The RBF kernel enabled the SVM to capture complex decision boundaries and achieve good classification performance. Feature scaling proved to be an essential preprocessing step because SVM relies on distance-based calculations and performs best when all features are on a similar scale. A major advantage of SVM is its ability to provide accurate classification for complex datasets using kernel functions. However, one limitation is that it becomes computationally expensive and slower when trained on large datasets or when selecting optimal hyperparameters.

---

## Repository Structure

```
Assignment-6/
│── Assignment-6.ipynb
│── README.md
```

---

## Author

**Name:** *Sree Parvathy*
**Topic:** Weather Condition Classification using Support Vector Machine (SVM) and Open-Meteo API
