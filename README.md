# Spam Email Detection Model

## Overview
This project implements a **Spam Email Detection Model** using **Logistic Regression**. It classifies emails as spam or ham (non-spam) based on text-based features extracted using **TF-IDF vectorization** and a **hash-based feature extraction method**.

## Features
- **Dataset:** Utilized a dataset of **5,572 emails** with labels (spam or ham).
- **Feature Engineering:** Applied **TF-IDF vectorization** and a **1,024-dimensional binary feature representation**.
- **Machine Learning Model:** Trained a **Logistic Regression** classifier.
- **Performance:** Achieved **95%+ accuracy** on test data.
- **Real-time Prediction:** Allows users to classify new email messages as spam or ham.

## Installation
### Prerequisites
Ensure you have Python installed along with the required libraries:
```bash
pip install numpy pandas scikit-learn matplotlib
```

## Usage
1. Clone the repository:
```bash
git clone https://github.com/your-repo/spam-email-detection.git
cd spam-email-detection

```
2. Enter a message for classification, and the model will predict if it's **Spam** or **Not Spam**.

## Model Training Steps
1. **Data Preprocessing**: Cleaned dataset by removing unnecessary columns and encoding labels.
2. **Feature Extraction**: Used **TF-IDF Vectorization** and a custom **hash-based feature extraction**.
3. **Model Training**: Applied **Logistic Regression** on the processed dataset.
4. **Evaluation**: Achieved over **95% accuracy** using an **80-20 train-test split**.

## Example Prediction
```python
input_txt = ["Congratulations! You have won a free prize!"]
input_fext = f_ext.transform(input_txt)
ans = model.predict(input_fext)
print("Spam mail" if ans[0] == 1 else "Not a Spam mail")
```
**Output:**
```
Spam mail
```



## License
This project is open-source and available under the MIT License.
