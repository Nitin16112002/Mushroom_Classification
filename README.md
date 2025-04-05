# 🍄 Mushroom Classifier

## 📌 Business Problem

A foraging supply company wants to develop a reliable tool to help amateur mushroom hunters and food suppliers distinguish between **edible** and **poisonous** mushrooms in the wild. Misidentification can lead to severe health risks or even fatalities.

Using mushrooms' physical characteristics, the company aims to build a machine learning classification model that can accurately classify the class.

---

## 📂 Dataset Overview

The dataset used in this project is derived from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/mushroom). It consists of 8124 instances of mushrooms with 22 categorical features, such as:

- **Cap**: shape, surface, and color
- **Odor** and **bruises**
- **Gill**: attachment, spacing, size, and color
- **Stalk**: shape, surface, and color
- **Ring**: number and type
- **Spore print color**
- **Habitat** and **population**

---

## 🧠 Models Used

The following ensemble models were trained and evaluated:

- `AdaBoostClassifier`
- `GradientBoostingClassifier`
- `XGBClassifier`

---

## 📊 Model Performance

| Model                   | Training Accuracy | Testing Accuracy | Cross-Validation Score | Training Time (s) |
|------------------------|-------------------|------------------|-------------------------|-------------------|
| AdaBoostClassifier     | 1.0000            | 1.0000           | 1.0000                  | 0.1053            |
| GradientBoosting       | 0.9997            | 0.9994           | 1.0000                  | 0.0518            |
| XGBClassifier          | 1.0000            | 1.0000           | 1.0000                  | 0.0806            |

All models performed exceptionally well, with nearly perfect scores across the board.

---

## 🔧 Preprocessing

- All categorical features were encoded using Label Encoding
- No missing values in the dataset
- Data split into training and test sets
- Cross-validation used for robust evaluation

---

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/mushroom-classifier.git
cd mushroom-classifier
