# Breast Cancer Decision Tree

## 📘 Overview
This project implements a **Decision Tree Classifier ** (without scikit-learn) to classify breast cancer patients as `Alive` or `Dead` based on the SEER dataset.  
The model uses **Gini impurity** for splits and is trained over 20 epochs, with accuracy and loss plotted against epochs.

---

## ⚙️ Requirements
Make sure you have the following Python libraries installed:
```
pip install numpy pandas matplotlib
```

---

## ▶️ Running Instructions
1. Open `Breast_Cancer_Decision_Tree.ipynb` in **Jupyter Notebook**.
2. Upload the dataset file **Breast_Cancer.csv** to the working directory .
3. Run all cells sequentially (`Shift + Enter`).

The notebook will:
- Load and clean the dataset.
- Encode categorical and target columns.
- Build a Decision Tree using Gini impurity (no external ML libraries).
- Train the tree for 20 epochs with randomized data splits.
- Display validation accuracy and loss for each epoch.
- Plot **Accuracy vs Epoch** and **Loss vs Epoch** graphs.

---

## 📊 Expected Output

### Console Output Example
```
Epoch 01: Train acc=0.85, Val acc=0.82, Val loss=0.18
Epoch 02: Train acc=0.86, Val acc=0.83, Val loss=0.17
...
Done training across epochs.
```

### Graph Output
Two plots will appear:
- **Accuracy vs Epoch**
- **Validation Loss vs Epoch**

---

## 🧠 Notes
- Maximum tree depth is limited to **5** (can be adjusted in code).
- Missing values: numerical → filled with mean, categorical → filled with mode.
- Target encoding: `Alive = 0`, `Dead = 1`.
- Validation loss = `1 - Validation Accuracy`.
- “Epochs” simulate retraining with different random splits each iteration.

---

## 📂 Files
- `notebook/Breasr_Cancer_one.ipynb` → Main implementation notebook.
- `result/Prediction.csv` → Prediction file.
- `model/DecisionTree_metrics.csv` → Model file.
- `data/Breast_Cancer.csv` → Dataset file.
- `README.txt` → This instruction file.

---

**Author:** Aritra Sarkar
