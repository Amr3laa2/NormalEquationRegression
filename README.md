# Normal Equation Regression

A from-scratch implementation of **Linear Regression using the Normal Equation** — solving for model weights directly via matrix algebra, with no gradient descent required. Applied to a real-world **apartment price prediction** dataset.

## What is the Normal Equation?

Instead of iteratively minimizing a cost function, the Normal Equation computes the optimal weights θ analytically in a single step:

```
θ = (XᵀX)⁻¹ Xᵀy
```

| Symbol | Meaning |
|---|---|
| `X` | Feature matrix |
| `y` | Target vector (prices) |
| `θ` | Model weights (solved directly) |

## Notebook

| File | Description |
|---|---|
| `ApartmentPricePrediction.ipynb` | Full pipeline: data loading, feature engineering, Normal Equation solution, and evaluation |

## Tech Stack

- Python
- NumPy (matrix operations)
- Pandas (data handling)
- Jupyter Notebook

## Getting Started

```bash
pip install numpy pandas jupyter
jupyter notebook ApartmentPricePrediction.ipynb
```

## When to Use the Normal Equation

- Small to medium datasets (no need to tune a learning rate)
- When you want an exact closed-form solution
- Teaching/understanding linear algebra behind regression
