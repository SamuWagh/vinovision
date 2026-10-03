# 🍷 VinoVision

### *Turning complex wine data into a visual story.*

Ever wondered how a dataset with many different features can be reduced to something we can actually **see and understand**?

**VinoVision** explores a wine dataset using **Principal Component Analysis (PCA)** to uncover patterns and visualize three different segments in a simple 2D space.

---

## 👀 Project Preview

### 📊 PCA Visualization

The project transforms the original wine features into two principal components and visualizes the three wine segments in a simple 2D plot.

<p align="center">
  <img src="images/pca_visualization.png" alt="VinoVision PCA Visualization" width="750">
</p>

> **From many wine features → 2 principal components → one clear visual story.** 🍷

### 🔬 Before PCA vs After PCA

| Original Data       | After PCA              |
| ------------------- | ---------------------- |
| Multiple features   | 2 Principal Components |
| Harder to visualize | Easy 2D visualization  |
| High-dimensional    | Reduced-dimensional    |

---

## 🔎 What is VinoVision?

Working with many features at once can make data difficult to interpret.

VinoVision takes those multiple features, **standardizes them**, and uses PCA to transform them into just two principal components:

```text
Wine Dataset
     ↓
Feature Standardization
     ↓
     PCA
     ↓
PC1 + PC2
     ↓
Visualize 3 Segments 🍷
```

The result is a simple visual representation that makes patterns in the dataset easier to explore.

---

## ✨ What I Did

* 📂 Loaded and explored the wine dataset
* ⚙️ Separated features and `Customer_Segment`
* 📏 Standardized the numerical features
* 🧠 Applied PCA using Scikit-learn
* 🔍 Reduced the data to 2 principal components
* 📊 Visualized the three segments using a scatter plot

---

## 🛠️ Tech Stack

**Python** · **Pandas** · **NumPy** · **Matplotlib** · **Scikit-learn** · **Jupyter Notebook**

---

## 📊 The Visualization

The final plot represents the dataset using:

**X-axis → Principal Component 1**
**Y-axis → Principal Component 2**

Each point represents an observation, allowing the distribution of the three segments to be visually explored.

---

## 🖼️ Adding the Preview Image

To display the project preview on GitHub:

### 1. Run the PCA visualization

Open `vinovision_pca.ipynb` and run the visualization cell.

### 2. Save the plot

Add this to the visualization code:

```python
plt.savefig("images/pca_visualization.png", dpi=300, bbox_inches="tight")
```

### 3. Create the images folder

Your repository should look like:

```text
VinoVision/
│
├── 📓 vinovision_pca.ipynb
├── 📊 wine.csv
├── 🖼️ images/
│   └── pca_visualization.png
└── 📄 README.md
```

### 4. Push it to GitHub

```bash
git add .
git commit -m "Add PCA visualization preview"
git push
```

GitHub will automatically render the image inside the README.

---

## 📁 Project Structure

```text
VinoVision/
│
├── 📓 vinovision_pca.ipynb
├── 📊 wine.csv
├── 🖼️ images/
│   └── pca_visualization.png
└── 📄 README.md
```

---

## 🚀 Run It Yourself

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/vinovision.git
cd vinovision
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open **`vinovision_pca.ipynb`** and run the cells.

---

## 💡 What I Learned

This project helped me understand how **dimensionality reduction** can turn a high-dimensional dataset into a form that is much easier to visualize and explore.

It also gave me practical experience with:

* Data preprocessing
* Feature scaling
* Principal Component Analysis
* Data visualization
* Working with Python ML libraries

---

## 🔮 What's Next?

VinoVision can be extended by:

* 📈 Exploring explained variance
* 📊 Adding a PCA scree plot
* 🖱️ Creating interactive visualizations
* 🤖 Applying classification algorithms to the transformed data
* 🔬 Comparing original features with PCA-based features

---

## 👩‍💻 Author

**Samruddhi Wagh**

> *Explore the data. Reduce the complexity. See the patterns.* 🍷

⭐ If you found VinoVision interesting, feel free to explore the notebook!
