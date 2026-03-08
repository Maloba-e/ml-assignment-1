# ml-assignment-1
### Google colab link: https://colab.research.google.com/drive/19sNEuG4wch3-AxWJYmkBAIj82YBB_JLi?usp=sharing

### 1. Exploratory Data Analysis (EDA)
*   **Missing Values**: The dataset is clean with no missing values.
*   **Class Distribution**: There is class imbalance with **115 NonToxic** samples and **56 Toxic** samples.
*   **Feature Complexity**: The dataset is high-dimensional, starting with **1,203 initial features**.

### 2. Data Preprocessing
*   **Target Encoding**: Successfully mapped labels to numerical values (NonToxic: 0, Toxic: 1).
*   **Feature Scaling**: Applied `StandardScaler` to all features to ensure consistency across the high-dimensional feature space.

### 3. Feature Selection (RFECV)
*   **Methodology**: Utilized Recursive Feature Elimination with Cross-Validation (RFECV) and a Random Forest estimator.
*   **Optimal Subset**: Determined that **1,143 features** provide the optimal balance for predictive accuracy.
*   **Finding**: Approximately 60 features were identified as redundant or noisy and removed to optimize model performance.

### 4. Model Training & Evaluation
*   **Overall Accuracy**: The final Random Forest model achieved **68.6% accuracy**.
*   **Recall Disparity**: The model shows a high recall for **NonToxic** cases (96%) but a low recall for **Toxic** cases (9%).
*   **ROC-AUC**: The model achieved an ROC-AUC score of **0.60**.

