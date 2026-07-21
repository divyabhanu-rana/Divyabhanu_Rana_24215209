# Practical 2: Implement a Single Neuron using Python and NumPy

## 🎯 Aim

To implement a **Single Artificial Neuron** using Python and NumPy with the **Sigmoid Activation Function** and train it to classify the **AND logic gate**. This experiment demonstrates how a neuron learns by adjusting its weights and bias using gradient-based updates.

---

## 📚 Main Topics Covered

- Artificial Neural Networks (ANN)
- Single Artificial Neuron
- Sigmoid Activation Function
- Binary Classification
- Weight & Bias Updates
- Probability Prediction
- NumPy

---

## 📖 Theory

An **Artificial Neuron** is the basic computational unit of an Artificial Neural Network. Similar to a biological neuron, it receives multiple inputs, processes them using weights and a bias, and produces an output through an activation function.

Unlike the Perceptron, which only produces binary outputs (0 or 1), this neuron uses the **Sigmoid Activation Function**, allowing it to generate probability values between **0 and 1**.

The mathematical model of a neuron is:

\[
z = \sum_{i=1}^{n} w_i x_i + b
\]

where

- **x** = Input Features
- **w** = Weights
- **b** = Bias

The weighted sum is passed through the Sigmoid Activation Function:

\[
\sigma(z)=\frac{1}{1+e^{-z}}
\]

The output represents the probability of belonging to the positive class.

---

## ⚙️ Code Concept

The implementation follows these steps:

1. Import NumPy.
2. Create the AND gate dataset.
3. Initialize weights and bias.
4. Define the Sigmoid activation function.
5. Perform forward propagation.
6. Compute prediction error.
7. Update weights and bias.
8. Repeat training for multiple epochs.
9. Predict outputs using the trained neuron.

The neuron gradually learns the relationship between the input features and the desired output by minimizing prediction errors during training.

---

## 🖥️ Sample Output

```text
Input: [0 0]
Output Probability: 0.05
Prediction: 0

Input: [0 1]
Output Probability: 0.24
Prediction: 0

Input: [1 0]
Output Probability: 0.25
Prediction: 0

Input: [1 1]
Output Probability: 0.66
Prediction: 1
```

---

## 🔍 Observations

- The neuron successfully learned the AND gate after multiple training iterations.
- Unlike the Perceptron, the model produced **probability values** instead of direct binary outputs.
- The Sigmoid activation function compressed every output between **0 and 1**, making it suitable for probability estimation.
- A threshold of **0.5** was used to convert probabilities into binary predictions.
- The weights and bias gradually converged toward values that minimized prediction error.
- This experiment demonstrates the role of activation functions in enabling smooth learning and gradient-based optimization.

---

## 🌍 Real-World Application

### Disease Risk Prediction

One of the most important applications of a Sigmoid-based neuron is **disease risk prediction** in healthcare.

Hospitals and diagnostic systems collect various patient parameters such as:

- Age
- Body Mass Index (BMI)
- Blood Pressure
- Blood Glucose Level
- Cholesterol
- Family Medical History

Each of these factors contributes differently toward predicting whether a patient is likely to develop a disease such as diabetes or heart disease. The neuron assigns weights to these features and computes a weighted sum, which is then passed through the Sigmoid activation function.

Instead of simply predicting **"Disease"** or **"No Disease"**, the neuron outputs a probability.

Example:

```text
Output = 0.87
```

This means there is an **87% probability** that the patient may have the disease.

Doctors can combine this probability with laboratory reports and medical history before making a final diagnosis. Such probabilistic predictions help prioritize high-risk patients, support clinical decision-making, and improve early disease detection.

Although modern healthcare systems employ deep neural networks with many hidden layers, the fundamental idea remains the same as demonstrated by this single neuron model.

---

## ✅ Conclusion

The Single Artificial Neuron was successfully implemented using Python and NumPy. The experiment demonstrated how a neuron computes weighted inputs, applies the Sigmoid activation function, and learns by adjusting its weights and bias during training. Unlike the Perceptron, the neuron provides probability-based predictions, making it suitable for many real-world binary classification problems. This experiment serves as an important stepping stone toward understanding deep neural networks.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Jupyter Notebook

---

## 🎓 Key Learning Outcomes

After completing this practical, the following concepts were understood:

- Working of an Artificial Neuron
- Difference between Perceptron and Sigmoid Neuron
- Importance of Activation Functions
- Probability-based Binary Classification
- Weight and Bias Optimization
- Gradient-based Learning
- Forward Propagation
