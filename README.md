# Perovskite Crystal Structure Classification using Machine Learning

This project applies machine learning techniques to classify perovskite crystal structures (Cubic, Orthorhombic, Rhombohedral, and Tetragonal) based on various elemental and spectral features.

## 🔍 Objective

- Classify perovskite crystals into distortion types using ML models.
- Analyze features such as ionic radii, bond lengths, and electronegativity differences.
- Identify key features influencing structural distortion.

## 🧪 Dataset

- Contains 200+ samples of perovskite materials.
- Features include:
  - Ionic radii
  - Electronegativity differences
  - Bond lengths
  - Goldschmidt tolerance factor (tG)
- Target variable: Crystal structure (encoded as 0–3).

## ⚙️ Methodology

1. **Data Preprocessing**
   - Dropped unnecessary columns and null values.
   - Converted object types to numeric.
   - Encoded target labels:
     - 0: Cubic
     - 1: Orthorhombic
     - 2: Rhombohedral
     - 3: Tetragonal

2. **Modeling**
   - Trained and evaluated:
     - Random Forest Classifier
     - XGBoost Classifier
     - Support Vector Machine (SVM)
   - Performed feature importance analysis.

## 📈 Results

| Model         | Accuracy | F1-Score |
|---------------|----------|----------|
| Random Forest | 82.2%    | 0.81     |
| XGBoost       | 82.6%    | 0.82     |

- XGBoost showed the best overall performance.
- Confusion matrix confirmed balanced classification across all four categories.
- Goldschmidt tolerance factor (tG) identified as the most significant feature.

## 🔍 Key Insights

- Feature importance analysis highlighted tG as the strongest predictor.
- Structural distortion is closely linked to elemental properties.

## 🚀 Future Work

- Hyperparameter tuning for improved performance.
- Explore advanced ensemble techniques like Gradient Boosting.
- Integrate domain knowledge for enhanced feature engineering.


## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

## 📬 Contact

For queries or collaboration: [YourEmail@example.com]  
LinkedIn: [Your LinkedIn Profile]

