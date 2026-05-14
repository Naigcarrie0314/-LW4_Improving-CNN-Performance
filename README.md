# 🧠 CNN Model Evaluation & Improvement Report


---

## 🔍 A. Model Evaluation Analysis

### 1. Weakest-performing classes
Based on the confusion matrix, the weakest-performing classes were the ones with lower diagonal values and more scattered predictions outside the diagonal. Some regions were frequently confused with similar-looking regions, which means the model had difficulty distinguishing features between those classes. A few classes showed lower prediction counts compared to others, indicating weaker recognition performance.

### 2. Precision, Recall, and F1-score variation
The Precision, Recall, and F1-score varied across the different region classes. Several classes achieved high scores close to 0.80–1.00, showing strong classification performance, while some classes had noticeably lower values around 0.40–0.70. This variation suggests that the model performed better on classes with clearer and more distinguishable features, while classes with similar patterns were harder to classify correctly.

### 3. Low recall meaning
Low recall means that the model failed to identify many actual samples belonging to a specific class. This resulted in a higher number of false negatives. In the confusion matrix, this can be observed when actual samples of one class were predicted as another class instead of their correct category.

### 4. AUC vs Accuracy
Accuracy measures the overall percentage of correct predictions, while AUC evaluates how well the model separates classes. From the results shown, some classes maintained strong AUC values even when their accuracy was not perfect, indicating that the model could still distinguish classes effectively. Therefore, AUC provides a more detailed assessment of classification capability than accuracy alone.

---

## ⚙️ B. Model Improvement

### 5. Data Augmentation
Data augmentation improved the model by increasing the diversity of training images. This helped the model generalize better to unseen data and reduced overfitting. The improved validation performance and more balanced class predictions suggest that augmentation contributed positively to the training process.

### 6. Batch Normalization
Batch Normalization stabilized the learning process and improved convergence during training. It normalized layer inputs, which helped the model train faster and achieve more consistent performance across epochs.

### 7. Dropout
Dropout reduced overfitting by randomly disabling neurons during training. This forced the network to learn more generalized features instead of memorizing the training data, which improved validation performance.

### 8. Early Stopping
Early Stopping prevented unnecessary training once the validation performance stopped improving. This helped avoid overfitting and preserved the model weights with the best validation results.

---

## 📊 C. Performance Comparison

### 9. Improvements observed
After applying the improvements, the model achieved better validation accuracy, lower validation loss, and more balanced Precision, Recall, and F1-scores across classes. The confusion matrix also showed stronger diagonal values, indicating more correct predictions.

### 10. Most impactful enhancement
Data augmentation appeared to provide the greatest improvement because it increased training diversity and helped the model recognize different image variations more effectively. This contributed to improved generalization and reduced misclassification.

### 11. Training vs Validation gap
Yes, the gap between training and validation performance decreased after the improvements. This indicates that the model generalized better and overfitting was reduced compared to earlier training results.
---

## 🔎 D. Explainability (Grad-CAM Integration)

### 12. Role of Grad-CAM
Grad-CAM helped visualize the regions of the image that influenced the model’s predictions. It highlighted the important areas the model focused on during classification, making the decision-making process easier to interpret.

### 13. Model focus improvement
Yes, the improved model appeared to focus more on relevant image regions rather than unrelated background areas. This indicates that the model learned more meaningful and discriminative features for classification.

### 14. Importance of Explainability
Explainability is important because it increases trust and transparency in AI systems. By understanding how the model makes decisions, researchers can identify errors, detect bias, and improve reliability. This is especially important in critical applications such as healthcare, security, and automated decision-making systems.

---

## 📎 Colab Notebook
👉 [Open in Google Colab](https://colab.research.google.com/drive/1VzO3Wntx_DMmEmofDXSuEMgNV1SX85ei?usp=sharing)
