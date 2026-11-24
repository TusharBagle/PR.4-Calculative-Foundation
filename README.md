# 🚀 PR.4 — Calculative Foundation
### Exploring the Mathematics Behind Data Science, Linear Algebra & Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.13+-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

<p align="center">
  <b>From Mathematical Theory to Practical Implementation.</b><br>
  Understanding how vectors, matrices, transformations and eigen-decomposition power modern data science.
</p>

---

## 📌 About The Project

**PR.4 — Calculative Foundation** is a hands-on Python project designed to explore the mathematical foundations of Data Science and Machine Learning through practical implementation.

Instead of learning mathematical concepts only through formulas, this project demonstrates how mathematical operations work using real numerical data, Python programming, NumPy and Pandas.

The project uses a dataset containing the academic scores of five students across three subjects:

- Mathematics
- Statistics
- Python

This dataset serves as the foundation for exploring vector representations, matrix operations, geometric transformations, dimensionality and eigen-decomposition.

**The main objective is to connect mathematical intuition with computational implementation.**

## 🎯 Project Objectives

- Understand vector representation and dimensional spaces.
- Implement L1 and L2 vector norms.
- Explore dot products, cross products and vector projections.
- Perform matrix addition, multiplication and transposition.
- Understand matrix inverses and determinants.
- Explore linear transformations and geometric interpretations.
- Understand dimensionality from 2D to higher-dimensional spaces.
- Calculate covariance matrices, eigenvalues and eigenvectors.
- Establish the mathematical foundation of Principal Component Analysis (PCA).

---

## 🧠 Concepts & Implementations

### PART A — Vector & Matrix Fundamentals

Explore the fundamental operations of vectors and understand how student performance can be represented mathematically.

| No. | Concept | Implementation |
|---|---|---|
| 01 | Vector Representation | Represent student scores as vectors |
| 02 | L1 & L2 Norms | Calculate vector magnitude |
| 03 | Dot Product | Measure vector alignment |
| 04 | Cross Product | Calculate perpendicular vectors in 3D |
| 05 | Vector Projection | Project one student's profile onto another |

**Key Mathematical Concepts:**

- Euclidean distance
- Manhattan norm
- Vector magnitude
- Angular relationships
- Orthogonality
- Projection and residuals

### PART B — Matrix Operations

Understand how matrices organize datasets and enable mathematical computations.

| No. | Concept | Implementation |
|---|---|---|
| 01 | Matrix Construction | Create a student-subject matrix |
| 02 | Matrix Addition | Apply a uniform bonus to scores |
| 03 | Matrix Multiplication | Calculate the subject Gram matrix |
| 04 | Transpose | Convert rows into columns |
| 05 | Matrix Inverse | Calculate the inverse of the Gram matrix |
| 06 | Determinant | Calculate the determinant of a square matrix |

**Key Mathematical Concepts:**

- Matrix dimensions
- Element-wise addition
- Matrix multiplication
- Identity matrices
- Invertibility
- Determinants and matrix rank

### PART C — Linear Transformations & Geometry

Explore the geometric interpretation of linear algebra.

| No. | Concept | Implementation |
|---|---|---|
| 01 | Linear Transformations | Transform vectors using matrices |
| 02 | Lines | Understand one-dimensional subspaces |
| 03 | Planes | Explore two-dimensional subspaces |
| 04 | Hyperplanes | Understand higher-dimensional geometry |
| 05 | Dimensionality | Explore 2D, 3D and higher-dimensional datasets |

**Key Mathematical Concepts:**

- Scaling transformations
- Geometric representation
- Coordinate spaces
- Linear subspaces
- Dimensionality and hyperplanes

### PART D — Eigenvalues & Decomposition

Explore how eigenvalues and eigenvectors reveal the underlying structure of a dataset.

| No. | Concept | Implementation |
|---|---|---|
| 01 | Covariance Matrix | Calculate relationships between subjects |
| 02 | Eigenvalues | Measure variance along principal directions |
| 03 | Eigenvectors | Identify principal directions |
| 04 | Eigen-decomposition | Decompose a symmetric covariance matrix |
| 05 | PCA Foundation | Understand dimensionality reduction |

**Key Mathematical Concepts:**

- Covariance
- Eigenvalues and eigenvectors
- Characteristic equations
- Symmetric matrices
- Positive semi-definite matrices
- Principal Component Analysis

---

## 📊 Dataset Overview

The project uses a sample dataset of five students and three academic subjects.

| Student | Mathematics | Statistics | Python |
|:---:|---:|---:|---:|
| S1 | 80 | 75 | 90 |
| S2 | 65 | 70 | 60 |
| S3 | 90 | 85 | 95 |
| S4 | 55 | 60 | 65 |
| S5 | 75 | 80 | 70 |

**Dataset Dimensions:**

- Number of observations: 5
- Number of features: 3
- Matrix dimensions: 5 × 3
- Mathematical space: R³ per student

The dataset is converted into a NumPy array for mathematical operations and initially organized using a Pandas DataFrame.

---

## 🔬 Selected Computational Results

The following results are obtained from the practical notebook.

**1. Vector Norms — Student S1**

```python
L1 = np.linalg.norm(S1, ord=1)
L2 = np.linalg.norm(S1, ord=2)
```

| Operation | Result |
|---|---:|
| L1 Norm | 245.00 |
| L2 Norm | 141.86 |

**2. Dot Product — S1 and S2**

```python
Dot = np.dot(S1, S2)
```

Result:

```text
15850
```

**3. Cross Product — S1 and S2**

```python
Cross = np.cross(S1, S2)
```

Result:

```text
[-1800  1050   725]
```

**4. Eigenvalues of the Covariance Matrix**

```python
Covariance = np.cov(X, rowvar=False)

Eigenvalues, Eigenvectors = np.linalg.eigh(Covariance)
```

Eigenvalues in descending order:

```text
[464.77191599
  51.95154564
   0.77653837]
```

Approximate variance explained:

| Principal Component | Variance Explained |
|---|---:|
| PC1 | 89.81% |
| PC2 | 10.04% |
| PC3 | 0.15% |

**Observation:** The first principal component captures approximately 89.81% of the total variance in this sample dataset.

This demonstrates how eigen-decomposition helps identify the most informative directions in data.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| NumPy | Numerical and linear algebra computations |
| Pandas | Dataset creation and manipulation |
| Jupyter Notebook | Interactive development and execution |

### Libraries Used

```python
import numpy as np
import pandas as pd
```

---

## ⚙️ Installation & Setup

Follow these steps to run the project locally.

**Step 1 — Clone the repository**

```bash
git clone https://github.com/TusharBagle/PR.4-Calculative-Foundation.git
```

**Step 2 — Navigate to the project directory**

```bash
cd PR.4-Calculative-Foundation
```

**Step 3 — Install dependencies**

```bash
pip install numpy pandas jupyter
```

**Step 4 — Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5 — Open the practical notebook**

```text
Practical_PR_4.ipynb
```

Run the notebook cells sequentially to explore the implementations and computational results.

---

## 📁 Repository Structure

```text
PR.4-Calculative-Foundation/
│
├── Practical_PR_4.ipynb
│
├── Part A - Theory of Vectors & Matrices.pdf
│
├── LICENSE
│
└── README.md
```

| File | Description |
|---|---|
| `Practical_PR_4.ipynb` | Practical Python implementation |
| `Part A - Theory of Vectors & Matrices.pdf` | Mathematical theory and explanations |
| `LICENSE` | MIT License |
| `README.md` | Project documentation |

---

## 💡 Learning Outcomes

Through this project, I explored how mathematical concepts translate into computational operations.

Some important takeaways:

1. **Vectors represent data:** Individual observations can be modeled as points in multidimensional spaces.
2. **Matrices organize information:** Datasets can be represented and manipulated using matrix operations.
3. **Geometry explains relationships:** Dot products, cross products and projections provide geometric interpretations of data.
4. **Transformations change representations:** Matrices can scale and transform vectors between coordinate spaces.
5. **Eigen-decomposition reveals structure:** Eigenvalues and eigenvectors help identify important directions of variation.
6. **Mathematics powers Machine Learning:** These concepts form the foundation of PCA, dimensionality reduction and many other ML techniques.

---

## 🚀 Real-World Applications

The mathematical foundations explored in this project are widely used in:

- **Data Science:** Numerical data representation and feature analysis.
- **Machine Learning:** Feature transformations and dimensionality reduction.
- **Artificial Intelligence:** Vector representations and mathematical optimization.
- **Statistics:** Covariance and relationships between variables.
- **Computer Vision:** Geometric transformations and multidimensional representations.
- **Information Retrieval:** Vector similarity and cosine similarity.

---

## 🔮 Future Enhancements

Potential improvements to extend this project:

- [ ] Implement complete PCA from scratch.
- [ ] Visualize vectors and transformations using Matplotlib.
- [ ] Create 2D and 3D geometric visualizations.
- [ ] Compare NumPy implementations with manual mathematical calculations.
- [ ] Explore Singular Value Decomposition (SVD).
- [ ] Add interactive visualizations for eigenvectors and principal components.
- [ ] Expand the dataset to explore higher-dimensional feature spaces.

---

## 📚 References & Learning Resources

- [NumPy Documentation](https://numpy.org/doc/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Python Documentation](https://docs.python.org/3/)
- [Jupyter Documentation](https://docs.jupyter.org/)
- [Linear Algebra — MIT OpenCourseWare](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/)

---

## 👨‍💻 Author

**Tushar Bagle**

Aspiring Data Science & Machine Learning Enthusiast

Interested in Python Programming, Statistics, Mathematics, Linear Algebra and Machine Learning.

<p align="center">
  <a href="https://github.com/TusharBagle">
    <img src="https://img.shields.io/badge/GitHub-TusharBagle-181717?style=for-the-badge&logo=github" />
  </a>
</p>

---

## 📜 License

This project is distributed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

<p align="center">
  <b>Mathematics is not just about solving equations — it is about understanding the structure behind data.</b>
  <br><br>
  ⭐ If you find this project interesting, consider giving it a star!
</p>
