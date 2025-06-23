# 🌸 Iris Dataset Classification using Decision Tree

This project demonstrates a **Decision Tree Classifier** on the famous [Iris flower dataset](https://archive.ics.uci.edu/ml/datasets/iris). It includes data visualization, preprocessing, model training, evaluation, and prediction.

## 📦 Dataset

The dataset contains 150 samples of iris flowers from three species:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

Each sample has 4 features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

## 📚 Requirements

Make sure you have the following libraries installed:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## 🚀 How to Run

1. Place `iris.csv` in your working directory.
2. Run the script in a Jupyter Notebook or any Python environment.

## 📊 Features

- **Data Visualization** using `seaborn.pairplot` and heatmap.
- **Data Preprocessing** using `LabelEncoder`.
- **Model Training** using `DecisionTreeClassifier`.
- **Evaluation** using classification report and confusion matrix.
- **Prediction** on new sample data.
- **Tree Visualization** using `plot_tree`.

## 📈 Model Accuracy

```
Accuracy: 1.0
```

✅ The model achieves **100% accuracy** on the test set (30% split).

## 🌳 Decision Tree Visualization

```python
mt.figure(figsize=(20,10))
plot_tree(dtree, feature_names=df.columns, precision=2, rounded=True, filled=True, class_names=target.values)
```

## 🔍 Predicting on New Data

```python
test = np.array([5.2, 1, 4, 2.5]).reshape(1, -1)
pred = dtree.predict(test)
print("Predicted Class:", New_data[int(pred[0])])
```

Output:
```
Predicted Class: Iris-viginica
```

## 📂 Project Structure

```
iris_project/
├── Iris.csv
├── file.ipynb
└── README.md
```

## 👨‍💻 Author

- [Your Name](#)
- [GitHub](#)

## 📝 License

This project is open-source and available under the MIT License.
