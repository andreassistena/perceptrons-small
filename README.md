# perceptrons-small
# Perceptrons as Logical Operators

This notebook explores how **perceptrons** (the simplest form of artificial neural networks) can be used to simulate basic logical operations such as **AND** and **NOT** using linear combinations and step functions.

---

## 🧠 Key Concepts

- **Perceptron Model**: A single-layer binary classifier that takes in input features, multiplies them by weights, adds a bias, and applies a step function to decide the output.

- **Linear Combination**:  
  \[
  \text{Output} = \text{Step}(w_1 \cdot x_1 + w_2 \cdot x_2 + b)
  \]

- **Activation Function**: A step function returning `1` if the linear combination ≥ 0, otherwise `0`.

---

## 🧪 Exercises Included

### ✅ 1. AND Operation

#### Task:
Use a perceptron to simulate the `AND` logic gate.

#### Inputs & Expected Outputs:
| Input 1 | Input 2 | Expected Output |
|---------|---------|-----------------|
| 0       | 0       | 0               |
| 0       | 1       | 0               |
| 1       | 0       | 0               |
| 1       | 1       | 1               |

#### Sample Weights:
```python
weight1 = 1
weight2 = 1
bias = -1.5
```

---

### ✅ 2. NOT Operation

#### Task:
Simulate a `NOT` gate by negating a single input in a two-variable environment.

#### Inputs & Expected Outputs:
| Input 1 | Input 2 | Expected Output |
|---------|---------|-----------------|
| 0       | 0       | 1               |
| 0       | 1       | 0               |
| 1       | 0       | 1               |
| 1       | 1       | 0               |

#### Sample Weights:
```python
weight1 = -1
weight2 = 0
bias = 0.5
```

---

## 📦 Requirements

- Python 3.x
- pandas
- Jupyter Notebook

Install with:
```bash
pip install pandas notebook
```

---

## 📚 Learning Notes

- This exercise reinforces the understanding of how linear models can perform binary classification.
- The perceptron can only model **linearly separable** functions.
- Combining multiple perceptrons (multi-layer networks) allows modeling of more complex logic like XOR.

---

## 📁 File Structure

- `Perceptrons as Logical Operators.ipynb` — The interactive notebook for practice.

---

## ✅ Next Steps

To deepen your understanding:
- Try modeling `OR` and `XOR` gates.
- Implement a 2-layer perceptron to solve XOR.
- Visualize the decision boundary using matplotlib.

---

## 🧠 Reference

- [Perceptron - Wikipedia](https://en.wikipedia.org/wiki/Perceptron)
- [scikit-learn Perceptron Class](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Perceptron.html)
