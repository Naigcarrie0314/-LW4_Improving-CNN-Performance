# 🧠 CNN Model Evaluation & Improvement Report


---

## 🔍 A. Model Evaluation Analysis

### 1. Weakest-performing classes
The weakest-performing classes were those with many misclassifications, shown by values spread outside the diagonal in the confusion matrix. These classes were often confused with similar classes, meaning the model had difficulty distinguishing their features.

### 2. Precision, Recall, and F1-score variation
Precision, Recall, and F1-score varied across classes. Some classes had high scores (around 0.80–0.90), indicating good performance, while others had lower scores (around 0.40–0.60), showing weaker classification. This indicates that the model performed unevenly across different classes.

### 3. Low recall meaning
Low recall means that the model failed to correctly identify many actual instances of a class. In other words, there are many false negatives, meaning the model is missing important data.

### 4. AUC vs Accuracy
Accuracy measures overall correctness, while AUC shows how well the model distinguishes between classes. A high AUC means the model can separate classes well even if accuracy is not perfect. Therefore, AUC provides a more detailed evaluation of performance compared to accuracy alone.

---

## ⚙️ B. Model Improvement

### 5. Data Augmentation
Data augmentation improved validation accuracy by increasing the diversity of training data. It helped the model generalize better and reduced overfitting.

### 6. Batch Normalization
Batch Normalization helps stabilize and speed up training by normalizing the inputs of each layer. It also improves model performance and makes training more efficient.

### 7. Dropout
Dropout reduces overfitting by randomly turning off some neurons during training. This forces the model to learn more robust and general features.

### 8. Early Stopping
Early Stopping prevents overfitting by stopping training when validation performance stops improving. This avoids unnecessary training and keeps the model from memorizing the data.

---

## 📊 C. Performance Comparison

### 9. Improvements observed
After modifying the model, validation accuracy increased, loss decreased, and predictions became more consistent.

### 10. Most impactful enhancement
Data augmentation contributed the most because it increased the variety of training data, which improved generalization and reduced overfitting.

### 11. Training vs Validation gap
Yes, the gap decreased. This means the model is no longer overfitting as much and performs more consistently on both training and validation data.

---

## 🔎 D. Explainability (Grad-CAM Integration)

### 12. Role of Grad-CAM
Grad-CAM helped by showing which parts of the image the model focused on when making predictions. This made the model’s decisions easier to understand.

### 13. Model focus improvement
Yes, the improved model focused more on relevant areas of the image rather than the background. This shows that the model learned more meaningful features.

### 14. Importance of Explainability
Explainability is important because it helps users trust the model, understand its decisions, and detect possible errors or bias. It is especially important in real-world applications like healthcare and security.

---

## 📎 Colab Notebook
👉 [Open in Google Colab](https://colab.research.google.com/drive/1VzO3Wntx_DMmEmofDXSuEMgNV1SX85ei?usp=sharing)
