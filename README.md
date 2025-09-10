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

## Quick Start

### Option A — Run in Google Colab (easiest)
1. Open Google Colab.
2. Upload `notebooks/supervised_vehicle_classification.ipynb`.
3. Run cells top-to-bottom.  
   *Most dependencies are preinstalled in Colab.*

### Option B — Run locally
```bash
# 1) Clone the repo
git clone <your-repo-url>
cd <repo-folder>

# 2) (Recommended) create a virtual environment
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# 3) Install dependencies
pip install -r requirements.txt

# 4) Start Jupyter and open the notebook
jupyter notebook  # or: jupyter lab

Usage

Open notebooks/supervised_vehicle_classification.ipynb.

Execute the sections in order:

1. Data Cleaning

2. Exploratory Data Analysis

3. Visualization (e.g., boxplots of numerical features)

4. Model Preparation (normalization, train/test split)

5. Model Go-Live (train RandomForest, predict on test data)

6. Evaluation (accuracy, classification report, confusion matrix/heatmap)

(Optional) Replace the dataset path with your own data to reuse the pipeline.

Requirements

Typical Python packages (see requirements.txt):
numpy
pandas
scikit-learn
matplotlib
seaborn

