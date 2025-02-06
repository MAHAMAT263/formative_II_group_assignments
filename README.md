# formative_II_group_assignments

# Neural Network Classification for Water Quality Potability

## 📌 Assignment Overview
This repository contains the implementation of a neural network classification model for predicting water quality potability. The project involves data preprocessing, model training, evaluation, and comparison of different architectures developed by each team member.

## 📂 Repository Contents
- **Notebook**: Contains the full implementation of the classification models using TensorFlow/Keras.
- **Training Summary Report**: Documents training results, observations, and model comparisons.
- **Video Submission**: Group video showcasing individual contributions, commits, training insights, and overall findings.
- **Summary Table**: Provides a structured comparison of model performances.

---

## 📊 Dataset
We use the **Water Quality and Potability** dataset from Kaggle, which consists of water quality parameters and a `Potability` label indicating whether the water is safe for consumption.

Dataset Link: [Water Quality and Potability](https://www.kaggle.com/datasets/uom190346a/water-quality-and-potability)

---

### ✅ **GitHub Repository Submission**
- The notebook with the implementation.
- Training summary report.
- Markdown documentation for easy navigation.

### 🎥 **Video Submission**
- Each team member explains their **contributions** and techniques used.
- Demonstration of commits and **training instances** from the report.
[Group Video](https://drive.google.com/drive/folders/1MfB5rXvLInY70BJNh4XIIpUoSBsaauYL?usp=drive_link)

### 📑 **Group Report**

- **Juliana vs. Liliane**:  
  My model outperformed Liliane’s, including a significantly higher F1 score (0.913 vs. 0.450). The inclusion of L2 regularization and the adaptive learning of the Adam optimizer allowed my model to generalize better, while Liliane’s model struggled due to the absence of L2 regularization and reliance on RMSprop.

- **Mahamat vs. Juliana**:  
  Juliana’s model performed better in terms of achieving higher test accuracy (88.7% vs. 68.7%) and F1 score (0.913 vs. 0.434). This difference stems from Juliana’s use of Adam, which converged more effectively than SGD, and her dropout rates, which better controlled overfitting.

- **Liliane vs. Mahamat**:  
  Mahamat’s model slightly outperformed Liliane’s model in terms of test accuracy (68.7% vs. 53.3%) and generalization, likely due to the inclusion of L2 regularization. Mahamat’s model also had a better early stopping patience. The criteria had a patience of 10 epochs, which allowed his model to stop training earlier when the validation loss plateaued, in contrast to Liliane’s model that had a patience of 50 epochs.





---

## 🔥 Challenges & Insights
- **Data Imbalance**: Strategies were explored to balance the dataset.
- **Optimization & Hyperparameters**: Different architectures and optimizers were tested for performance improvements.
- **Model Overfitting**: Regularization and dropout were used to prevent overfitting.

---

## 📝 Summary Table
| Member Name | Regularization Technique | Optimizer | Early Stopping Criteria | Dropout Rate | Train Accuracy | Test Accuracy | F1 Score |
|-------------|------------------------|-----------|-------------------------|--------------|----------------|--------------|---------|
| Mahamat    | L2 Regularization + Dropout | SGD (lr=0.01, momentum=0.9) | Monitor: val_loss, Patience: 10 | 0.3 (Layer 1), 0.3 (Layer 2) | 0.696 | 0.687 | 0.434 |
| kayitesi Liliane    | Dropout | RMSprop | Monitor: val_loss, Patience: 50 |0.3 (Layer 1), 0.2 (Layer 2) | 0.663	| 0.533 | 	0.450 |
| Juliana C. Holder   | L2 Regularization | Adam | Monitor: val_loss, Patience: 7 | 0.25 (Layer 1), 0.4 (Layer 2) | 0.897 | 0.887 | 0.913 |
