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

# Model Performance Comparisons

## Comparative Analysis

### Juliana (Best Overall Performance)
When comparing with Liliane's model, my F1 score was higher (0.590 vs 0.450) and I achieved better test accuracy (64.6% vs 53.3%). The performance came from my choice of combining L2 regularization with the Adam optimizer, which provided better parameter updates compared to Liliane's RMSprop approach. When looking at Mahamat's model, while he achieved excellent generalization, my model still produced better overall metrics with a higher F1 score (0.590 vs 0.434). The key difference was my use of Adam optimizer instead of SGD with momentum, which allowed for more adaptive learning rates and better convergence.

### Mahamat (Best Generalization)
While my F1 score (0.434) was lower than my teammates, my model achieved the best generalization performance with nearly identical train and test accuracies (0.696/0.687). Compared to Liliane's model, my combined L2 and dropout regularization strategy proved more effective than her dropout-only approach, as evidenced by my minimal train-test accuracy gap (0.009 vs 0.130). When looking at Juliana's model, although she achieved higher absolute metrics, my model demonstrated better stability and generalization.

### Liliane (Second-Best F1 Score)
My model achieved the second-best F1 score (0.450) among the team. While Juliana's model showed higher metrics overall, my RMSprop optimizer still managed to achieve decent training performance (0.663). When comparing with Mahamat's model, my higher F1 score (0.450 vs 0.434) shows the potential of my approach, though the larger train-test accuracy gap indicates room for improvement.
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
| Juliana C. Holder   | L2 Regularization | Adam | Monitor: val_loss, Patience: 7 | 0.25 (Layer 1), 0.4 (Layer 2) | 0.724 | 0.646 | 0.590 |
