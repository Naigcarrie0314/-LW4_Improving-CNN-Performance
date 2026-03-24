Google Colab link https://colab.research.google.com/drive/1VzO3Wntx_DMmEmofDXSuEMgNV1SX85ei?usp=sharing


GUIDE QUESTIONS (Student Explanation & Reflection) A. Model Evaluation Analysis

What were the weakest-performing classes based on the confusion matrix?
  -The weakest-performing classes were those with many misclassifications, shown by values spread outside the diagonal in the confusion matrix. These classes were often confused with similar classes, meaning the model had difficulty distinguishing their features.
How did Precision, Recall, and F1-score vary across classes?
  -Precision, Recall, and F1-score varied across classes. Some classes had high scores (around 0.80–0.90), indicating good performance, while others had lower scores (around 0.40–0.60), showing weaker classification. This indicates that the model performed unevenly across different classes.
What does a low recall indicate in your model?
  -Low recall means that the model failed to correctly identify many actual instances of a class. In other words, there are many false negatives, meaning the model is missing important data.
How does AUC score reflect model performance compared to accuracy?
  -Accuracy measures overall correctness, while AUC shows how well the model distinguishes between classes. A high AUC means the model can separate classes well even if accuracy is not perfect. Therefore, AUC provides a more detailed evaluation of performance compared to accuracy alone.

B. Model Improvement
6. How did data augmentation affect validation accuracy? 
  -Data augmentation improved validation accuracy by increasing the diversity of training data. It helped the model generalize better and reduced overfitting.
  -Batch Normalization helps stabilize and speed up training by normalizing the inputs of each layer. It also improves model performance and makes training more efficient.
7. Why is Batch Normalization important in CNNs?
  -Batch Normalization is important in CNNs because it normalizes the input of each layer, which helps make training faster and more stable. It reduces the problem of changing data distribution inside the network (internal covariate shift), allowing the model to learn more efficiently.
8. What role did Dropout play in improving your model? 
  -Dropout reduces overfitting by randomly turning off some neurons during training. This forces the model to learn more robust and general features.
9. How did Early Stopping prevent overfitting?
  -Early Stopping prevents overfitting by stopping training when validation performance stops improving. This avoids unnecessary training and keeps the model from memorizing the data.

C. Performance Comparison 
10. What improvements were observed after modifying the model? 
  -After modifying the model, validation accuracy increased, loss decreased, and predictions became more consistent.
11. Which enhancement contributed the most to performance improvement? Why?
  -Data augmentation contributed the most because it increased the variety of training data, which improved generalization and reduced overfitting.
12. Did the gap between training and validation accuracy decrease? Explain.
  -Yes, the gap decreased. This means the model is no longer overfitting as much and performs more consistently on both training and validation data.

D. Explainability (Grad-CAM Integration)
13. How did Grad-CAM help in understanding model predictions?
  -Grad-CAM helped by showing which parts of the image the model focused on when making predictions. This made the model’s decisions easier to understand.
14. Did the improved model focus on more relevant regions? Provide evidence.
  -Yes, the improved model focused more on relevant areas of the image rather than the background. This shows that the model learned more meaningful features.
15. Why is explainability important in real-world AI applications?
  -Explainability is important because it helps users trust the model, understand its decisions, and detect possible errors or bias. It is especially important in real-world applications like healthcare and security.
