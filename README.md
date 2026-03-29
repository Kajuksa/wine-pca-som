# 🍷 Wine Quality Analysis – PCA, SOM & UMAP

> **Técnicas Matemáticas para Big Data – Project M3**  
> Unsupervised dimensionality reduction and clustering applied to physicochemical wine data

---

## 📌 Problem Statement

Wine quality assessment is traditionally performed by human experts — a process that is subjective, slow, and costly. This project applies **data-driven unsupervised learning** techniques to analyze wine quality objectively using physicochemical measurements (acidity, alcohol, sulphates, pH, etc.).

---

## 🧠 Approach & Methods

Three complementary unsupervised methods are applied and compared:

| Method | Purpose |
|--------|---------|
| **PCA** (Principal Component Analysis) | Dimensionality reduction, variance preservation |
| **SOM** (Self-Organizing Map) | Topological clustering, visual neighbourhood mapping |
| **UMAP + HDBSCAN** | Non-linear projection + automatic cluster detection |

### Workflow
1. Load and standardize the Wine Quality dataset
2. Apply PCA to reduce features to principal components
3. Train a SOM to map data onto a 2D grid
4. Apply UMAP for non-linear projection, then HDBSCAN for clustering
5. Compare and validate results across all three methods

---

## 📂 Project Structure

```
wine-pca-som/
│
├── M3G3.ipynb            # Main notebook with full analysis
├── README.md             # This file
└── requirements.txt      # Python dependencies
```

---

## 🗃️ Dataset

**Wine Quality Dataset** (UCI Machine Learning Repository)  
- Physicochemical features: fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol  
- Target: quality score (0–10)  
- [Download here](https://archive.ics.uci.edu/ml/datasets/wine+quality)

---

## ⚙️ Setup & Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/wine-pca-som.git
cd wine-pca-som

# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook M3G3.ipynb
```

---

## 📊 Key Results

- **PCA** successfully reduced 11 features while preserving the majority of variance
- **SOM** revealed topological clusters aligned with wine quality scores
- **UMAP + HDBSCAN** identified natural groupings invisible to linear methods
- All three methods converged on consistent quality-based cluster patterns

---

## 👥 Authors

| Name | Student No. |
|------|-------------|
| Yangiboev Iftikhor | 130832 |
| Kajus Misevičius | 130237 |
| Maria João Machado Sardinha | 108756 |

---

## 📄 License

Developed for academic purposes as part of the *Técnicas Matemáticas para Big Data* course.
