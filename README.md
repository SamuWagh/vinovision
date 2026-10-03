# 🍷 VinoVision

### *See the data. Find the pattern. Understand the wine.*

What if a dataset with many different wine characteristics could be transformed into a simple visual story?

**VinoVision** is a Python-based data analysis project that uses **Principal Component Analysis (PCA)** to reduce multiple wine features into just two dimensions and visualize patterns across three customer segments.

---

## 🧠 The Idea

Real-world datasets can contain many features, making them difficult to visualize directly.

VinoVision simplifies the problem:

```text
🍷 Wine Dataset
       ↓
📊 Explore the Data
       ↓
📏 Standardize Features
       ↓
🧠 Apply PCA
       ↓
🔍 Reduce Dimensions
       ↓
📈 Visualize 3 Segments
```

Instead of looking at a large number of features separately, PCA helps represent the data using **Principal Component 1** and **Principal Component 2**.

---

## ✨ What Happens Inside?

### 01 — Explore

The wine dataset is loaded and examined to understand its features and structure.

### 02 — Prepare

The feature columns are separated from the `Customer_Segment` column and standardized using `StandardScaler`.

### 03 — Transform

**PCA** is applied using Scikit-learn with:

```python
PCA(n_components=2)
```

This reduces the dataset to two principal components.

### 04 — Visualize

The transformed data is plotted in a 2D scatter plot, making the distribution of the three segments easier to explore.

---

## 📊 Why PCA?

Imagine having a dataset with many dimensions.

You can't easily visualize all of them at once.

PCA creates new dimensions that capture important variation in the data, allowing us to represent a high-dimensional dataset in a simpler form.

```text
Many Features
     ↓
   PCA
     ↓
   PC1 ─────── PC2
     ↓
  2D View
```

This makes complex data easier to **explore, interpret, and visualize**.

---

## 🛠️ Tech Stack

| Tool                | Purpose                       |
| ------------------- | ----------------------------- |
| 🐍 Python           | Core programming              |
| 🐼 Pandas           | Data handling                 |
| 🔢 NumPy            | Numerical operations          |
| 📊 Matplotlib       | Data visualization            |
| 🤖 Scikit-learn     | Standardization & PCA         |
| 📓 Jupyter Notebook | Development & experimentation |

---

## 📈 What the Visualization Shows

The final visualization uses:

* **X-axis:** Principal Component 1
* **Y-axis:** Principal Component 2
* **Groups:** Three customer segments

Each point represents an observation from the wine dataset.

The visualization provides a way to visually explore whether observations from different segments show distinct patterns after dimensionality reduction.

> **The goal isn't just to reduce dimensions — it's to make the data easier to see.**

---

## 📁 Project Structure

```text
VinoVision/
│
├── 📓 vinovision_pca.ipynb
├── 📊 wine.csv
└── 📄 README.md
```

---

## 🚀 Run VinoVision Locally

### 1. Clone the repository

```bash
git clone https://github.com/SamuWagh/vinovision.git
cd vinovision
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open the project

Open:

```text
vinovision_pca.ipynb
```

Run the notebook cells to reproduce the analysis and visualization.

---

## 💡 What I Learned

Through VinoVision, I gained practical experience with:

* Data exploration
* Feature selection
* Data standardization
* Dimensionality reduction
* Principal Component Analysis
* Data visualization
* Working with Scikit-learn

Most importantly, I learned how a complex dataset can be transformed into a much simpler visual representation.

---

## 🔮 Future Ideas

VinoVision could be taken further by:

* 📈 Analyzing explained variance
* 📊 Adding a PCA scree plot
* 🖱️ Creating interactive visualizations
* 🤖 Applying classification algorithms
* 🔬 Comparing PCA features with the original features
* 📉 Exploring different dimensionality-reduction techniques

---

## 👩‍💻 Author

**Samruddhi Wagh**

A small project exploring how **data transformation can turn complexity into clarity.**

> 🍷 **Explore → Reduce → Visualize → Understand**

---

⭐ **If you found VinoVision interesting, feel free to explore the notebook and experiment with the data.**

