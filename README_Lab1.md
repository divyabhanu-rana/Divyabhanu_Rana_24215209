# Practical 1: Simulate a Perceptron using NumPy

## 🎯 Aim

To implement a **Perceptron**, the simplest form of an Artificial Neural Network (ANN), using NumPy and train it to correctly classify the **AND logic gate** using the Perceptron Learning Algorithm.

---

## 📚 Main Topics Covered

- Artificial Neural Networks (ANN)
- Perceptron Model
- Binary Classification
- Step Activation Function
- Perceptron Learning Rule
- Weight & Bias Updates
- NumPy

---

## 📖 Theory

The **Perceptron** is one of the earliest neural network models introduced by Frank Rosenblatt in 1958. It consists of a single neuron that receives multiple input features, multiplies each feature by its corresponding weight, adds a bias, and passes the result through an activation function.

Mathematically,

\[
Output = Step\left(\sum_{i=1}^{n} w_i x_i + b\right)
\]

where:

- **x** = input features
- **w** = weights
- **b** = bias
- **Step()** = activation function

The perceptron learns by iteratively adjusting its weights whenever it makes an incorrect prediction.

---

## ⚙️ Code Concept

The implementation follows these steps:

1. Import the NumPy library.
2. Create the AND gate dataset.
3. Initialize weights and bias.
4. Define the Step Activation Function.
5. Train the perceptron using the Perceptron Learning Rule.
6. Update weights and bias based on prediction error.
7. Repeat training for multiple epochs.
8. Test the trained perceptron.

---

## 🖥️ Sample Output

```text
Final Weights: [0.2 0.1]
Final Bias: -0.2

Predictions:

[0 0] → 0
[0 1] → 0
[1 0] → 0
[1 1] → 1
```

---

## 🔍 Observations

- The perceptron initially produced incorrect predictions because all weights were initialized to zero.
- During training, the weights and bias were updated whenever the prediction differed from the expected output.
- After several epochs, the model correctly classified every AND gate input.
- The experiment demonstrates how a neural network gradually learns from data rather than relying on manually written rules.
- The perceptron successfully solves **linearly separable** problems but cannot solve **non-linearly separable** problems such as the XOR gate.

---

## 🌍 Real-World Application

### Spam Email Classification

One of the earliest applications of the perceptron is **binary email classification**, where emails are categorized as either **Spam** or **Not Spam**.

A spam detection system extracts several features from every incoming email, such as:

- Presence of suspicious keywords (e.g., "Congratulations", "Free", "Lottery")
- Number of hyperlinks
- Presence of unknown attachments
- Sender reputation score
- Frequency of promotional phrases

Each feature is assigned a weight based on its importance. The perceptron calculates a weighted sum of these features, adds a bias, and applies the Step Activation Function to determine the final class.

If the computed value exceeds a threshold, the email is marked as **Spam**; otherwise, it is classified as **Not Spam**.

Although modern spam filters use advanced deep learning algorithms, the perceptron introduces the core concept of **binary classification**, which remains fundamental to machine learning systems today.

---

## ✅ Conclusion

The Perceptron was successfully implemented using NumPy and trained to classify the AND logic gate. This experiment demonstrated how a neural network learns by updating its weights and bias based on prediction errors. Despite its limitations to linearly separable data, the perceptron forms the foundation of modern neural networks and binary classification algorithms.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Jupyter Notebook
