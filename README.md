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
- **Summary of findings** and their significance.

### 📑 **Group Report**
- **Training summaries** for each model attempted by team members.
- **Results and conclusions** from the experiments.
- **Insights and challenges** faced by each member.
- **Summary Table** comparing model architectures and performances.



---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone <repository_link>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

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
| Member 3    | TBD | TBD | TBD | TBD | TBD | TBD | TBD |
