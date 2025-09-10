# Classification-model-supervised-

# Supervised Vehicle Classification (Colab)

This project builds a **supervised classification model** to predict the vehicle class (*car*, *van*, *bus*).  
The pipeline covers **data cleaning**, **exploratory data analysis (EDA)**, **visualization** of numerical features, **preprocessing** (normalization), a **train/test split**, model training with **RandomForestClassifier (100 trees)**, and an evaluation using **accuracy**, **classification report**, and a **confusion-matrix heatmap**.

**Result:** Test accuracy of **96.93%**. *Bus* and *Van* are recognized very reliably (**recall = 1.00**), with minor misclassifications among some *cars*.  
A “Go-Live” section shows how to apply the trained model to new, unseen data.

---

## Project Structure

├─ notebooks/
│ └─ supervised_vehicle_classification.ipynb # main Colab/Notebook
├─ src/ # optional helper functions
├─ data/ # sample or external data (keep large/sensitive data out of Git)
├─ figures/ # saved plots (optional)
├─ requirements.txt
├─ .gitignore
└─ README.md


---

Requirements

Typical Python packages (see requirements.txt):
numpy
pandas
scikit-learn
matplotlib
seaborn

