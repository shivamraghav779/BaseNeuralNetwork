# Neural Network from Scratch

This project implements a simple neural network from scratch using pure Python — without relying on any machine learning frameworks.

The goal is to understand the core mechanics behind neural networks, including forward propagation, activation functions, error calculation, and weight updates via gradient descent.

---

## Overview

This is a single-layer neural network trained on a small dataset to learn a basic pattern.

It demonstrates how a neural network:

* Takes input features
* Applies weights
* Passes through an activation function
* Computes error
* Adjusts weights iteratively to improve predictions

---

## Key Concepts Implemented

* Weighted sum of inputs
* Sigmoid activation function
* Forward propagation
* Error (loss) calculation
* Backpropagation (gradient descent)
* Iterative training loop

---

## How It Works

### 1. Initialization

* Weights are randomly initialized between -1 and 1
* A fixed random seed ensures reproducibility

### 2. Forward Propagation

* Inputs are multiplied by weights and summed
* Output is passed through a sigmoid activation function

### 3. Error Calculation

* Error = Actual Output - Predicted Output

### 4. Backpropagation

Weights are updated using the rule:

```
adjustment = input × error × sigmoid_derivative(output)
```

This process is repeated for multiple iterations to minimize the error.

---

## Training Data

The model is trained on a small dataset:

```
training_set_examples = [
    {"inputs": [0, 0, 1], "output": 0},
    {"inputs": [1, 1, 1], "output": 1},
    {"inputs": [1, 0, 1], "output": 1},
    {"inputs": [0, 1, 1], "output": 0}
]
```

---

## Running the Project

### 1. Clone the repository

```
git clone https://github.com/your-username/neural-network-from-scratch.git
cd neural-network-from-scratch
```

### 2. Run the script

```
python neural_network.py
```

---

## Example Output

```
Random starting weights: [...]
New weights after training: [...]
Prediction for [1, 0, 0] -> 0.99
```

---

## Why This Project Matters

Understanding neural networks at this level helps in:

* Building intuition for deep learning systems
* Debugging model behavior
* Designing more complex architectures
* Working effectively with frameworks like PyTorch or TensorFlow

It shifts the mindset from using tools to understanding systems.

---

## Next Steps

Possible improvements and extensions:

* Add multiple layers (Deep Neural Network)
* Implement different activation functions (ReLU, Tanh)
* Add learning rate control
* Visualize loss over time
* Extend to real-world datasets

---

## Author

Shivam Raghav
AI Engineer | Machine Learning | LLM Systems

---

## License

This project is open-source and available under the MIT License.
