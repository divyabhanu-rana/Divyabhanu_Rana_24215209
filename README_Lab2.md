# Practical 2: Implement a Single Neuron Model Manually using Python

## Aim

To implement a **single artificial neuron** using Python and NumPy with the **Sigmoid activation function** for binary classification of the AND logic gate.

---

## Main Topic

- Artificial Neuron
- Sigmoid Activation Function
- Binary Classification
- Weight Update
- Manual Neural Network Implementation

---

## Code Concept

This program manually simulates the working of a single artificial neuron.

The implementation includes:

- Initializing weights and bias.
- Computing the weighted sum of inputs.
- Applying the Sigmoid activation function.
- Calculating prediction error.
- Updating weights and bias iteratively.
- Predicting outputs after training.

Unlike a perceptron, the neuron uses the **Sigmoid activation function**, which produces probability values between 0 and 1.

---

## Output

```text
Input: [0 0]
Output: 0.0504
Prediction: 0

Input: [0 1]
Output: 0.2416
Prediction: 0

Input: [1 0]
Output: 0.2462
Prediction: 0

Input: [1 1]
Output: 0.6624
Prediction: 1
```

---

## Observations

- The neuron successfully learned the AND gate.
- The Sigmoid function generated outputs between 0 and 1.
- A threshold value of 0.5 was used to classify outputs into binary classes.
- Training gradually reduced prediction error and improved accuracy.

---

## Conclusion

The single neuron model was successfully implemented using Python and NumPy. The experiment demonstrated how weights, bias, and the Sigmoid activation function work together to perform binary classification through iterative learning.
