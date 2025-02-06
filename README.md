
**Breast Cancer Data Analysis**

The goal of this project is to build a model that predicts whether a patient has malignant cancer. The dataset used for this analysis is sourced from the UIC machine learning database.

The predictor variables in the dataset include Clump Thickness, Cell Size, Cell Shape, Marginal Adhesion, Single Epithelial Cell Size, Bare Nuclei, Normal Nucleoli, Bland Chromatin, and Mitoses. The target variable, which the model aims to predict, is the cancer class, classified as either benign (2) or malignant (4).

**Model Development**

The original dataset was used, but the number of categories for each variable was significantly reduced by grouping them into 2, 3, or 4 clusters where appropriate. A logistic regression model was developed with an emphasis on recall, as identifying every positive case is crucial. The model achieved an accuracy score of 96% on the training data and 97% on the test data, with recall, precision, and F1 scores of 96%. The ROC AUC was 97%.

**Conclusion**

The dataset analysis revealed that certain features are more common in benign or malignant cases. For example, **Marginal Adhesion** and **Single Epithelial Cell Size** of 4 or higher were predominantly seen in malignant cases, while benign cases were mainly observed in categories 1, 2, and 3 for these features.

The **number of normal nuclei** was found to be lower in malignant cases in categories 1, 2, and 3, and higher in categories 4 and above. Conversely, benign cases exhibited the opposite pattern. **Bland Chromatin** was more frequently observed in malignant cases in categories 3 and above.

In terms of **Mitosis**, benign cases were mostly found in category 1, with few in category 2 and higher. Malignant cases were prevalent across categories 1 to 4, leading to the suggestion of grouping categories 2 and above for modeling, with a cutoff set at 1.

Regarding **Clump Thickness**, benign cases were spread across all categories, whereas malignant cases had lower thickness values in the first four categories. For **Cell Size**, most benign cases were observed in categories 1, 2, and 3, while malignant cases were more common in categories above 4. A similar pattern was found for **Cell Shape**, where benign cases were primarily in categories 1, 2, and 3, while malignant cases increased in categories 3 and higher, especially in category 5. Finally, **Bare Nuclei** showed that most benign cases were found in category 1, with some in categories 2 and 3, whereas malignant cases were more frequent in categories 3 and higher, particularly in category 10.
Outputs:
![image](https://github.com/user-attachments/assets/8aa3d7cd-c18b-4135-bdc5-ece4e708401c)

![image](https://github.com/user-attachments/assets/05a7a657-f53e-4d1e-8573-aa462bb92ea6)


