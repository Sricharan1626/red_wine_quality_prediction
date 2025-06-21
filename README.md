# Red Wine Quality Prediction

This repository provides a machine learning solution for predicting the quality of red wine using various chemical properties. The model is trained on the popular "Wine Quality" dataset and is serialized as `trained.zip` (saved using `joblib`) for easy reuse and deployment.

## Features

- Data preprocessing and feature engineering
- Model training and evaluation
- Saved trained model (`trained.zip`)
- Example code for loading and using the model

---

## Getting Started

### 1. Clone the Repository

To get a local copy of the code, run:

```bash
git clone https://github.com/Sricharan1626/red_wine_qualtiy_prediction.git
cd red_wine_qualtiy_prediction
```

### 2. Install Dependencies

Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```

Ensure you have `joblib` and `scikit-learn` installed:

```bash
pip install joblib scikit-learn
```

---

## Using the Trained Model

The trained model is saved as `trained.zip` in the repository. You can load and use it as follows:

```python
import joblib

# Load the trained model
model = joblib.load('trained.zip')

# Example: Predict quality for a new wine sample
# Replace the example features with your own data
sample = [[7.4, 0.7, 0.0, 1.9, 0.076, 11.0, 34.0, 0.9978, 3.51, 0.56, 9.4]]
prediction = model.predict(sample)
print(f"Predicted wine quality: {prediction[0]}")
```

---

## Project Structure

```
red_wine_qualtiy_prediction/
│
├── trained.zip            # Trained model saved with joblib
├── requirements.txt       # Python dependencies
├── <other scripts and notebooks>
└── README.md
```

---

## Dataset

The project uses the [Wine Quality Dataset](https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009#:~:text=get_app,chevron_right) from the UCI Machine Learning Repository.

---

## Contributing

Pull requests are welcome! Please open an issue first for major changes.

---

## Acknowledgments

- UCI Machine Learning Repository for the dataset
- scikit-learn for machine learning tools
