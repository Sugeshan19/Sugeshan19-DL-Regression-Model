
# 1D Linear Regression Model (PyTorch)

A concise deep-learning style regression project that demonstrates how to train a simple linear model in PyTorch on synthetic 1D data.

## Overview

This project builds and trains a `torch.nn.Linear(1, 1)` model to learn a noisy linear relationship:

`y = 2x + 1 + noise`

The workflow is implemented in a single notebook (`ex1.ipynb`) and includes:

- Synthetic dataset generation
- Data visualization
- Model initialization
- Training with Mean Squared Error (MSE) and SGD
- Loss tracking across epochs
- Final best-fit line visualization

## Project Structure

```text
.
|-- ex1.ipynb      # End-to-end notebook for data generation, training, and plots
`-- README.md      # Project documentation
```

## Tech Stack

- Python 3.9+
- PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook (or VS Code Notebook support)

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Sugeshan19/Sugeshan19-DL-Regression-Model.git
cd Sugeshan19-DL-Regression-Model
```

### 2. Install dependencies

```bash
pip install torch numpy matplotlib notebook
```

### 3. Run the notebook

Option A (Jupyter):

```bash
jupyter notebook
```

Then open `ex1.ipynb` and run all cells.

Option B (VS Code):

- Open the folder in VS Code
- Open `ex1.ipynb`
- Select a Python interpreter
- Run all notebook cells

## Training Details

- Input samples: `X = [1, 2, ..., 70]`
- Noise: integer random values in `[-8, 8]`
- Target: `y = 2X + 1 + e`
- Model: `nn.Linear(1, 1)`
- Loss: `nn.MSELoss()`
- Optimizer: `torch.optim.SGD`
- Learning rate: `0.0001`
- Epochs: `50`

## Expected Output

When you run the notebook, you should see:

- A scatter plot of generated noisy linear data
- Epoch-wise logs for loss, weight, and bias
- A loss curve showing optimization progress
- The final best-fit line over the data

## Learning Goal

This project is a beginner-friendly reference for understanding the core mechanics of supervised learning in PyTorch:

- How data and labels are created
- How parameters are updated via backpropagation
- How model fit is interpreted visually

## License

This project is available for educational and personal use.

