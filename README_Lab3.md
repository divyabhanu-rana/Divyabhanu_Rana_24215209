# Practical 3: Implement a Feedforward Neural Network using TensorFlow

## Aim

To implement a **Feedforward Neural Network (FNN)** using TensorFlow (Keras) for binary classification of the AND logic gate.

---

## Main Topic

- Feedforward Neural Network (FNN)
- TensorFlow
- Keras Sequential Model
- Dense Layers
- ReLU Activation Function
- Sigmoid Activation Function
- Binary Classification

---

## Code Concept

This program implements a Feedforward Neural Network using TensorFlow's Keras API.

The implementation consists of the following steps:

- Import TensorFlow and NumPy libraries.
- Create the AND gate dataset.
- Build a Sequential neural network model.
- Add an input layer.
- Add one hidden Dense layer with ReLU activation.
- Add one output Dense layer with Sigmoid activation.
- Compile the model using the Adam optimizer and Binary Crossentropy loss.
- Train the network on the dataset.
- Evaluate the model.
- Predict outputs for all input combinations.

The neural network automatically learns the optimal weights using backpropagation during training.

---

## Output

```text
Training Accuracy: 100.0%

Predictions:

Input: [0 0]
Output: 0.0000
Prediction: 0

Input: [0 1]
Output: 0.0001
Prediction: 0

Input: [1 0]
Output: 0.0038
Prediction: 0

Input: [1 1]
Output: 0.9998
Prediction: 1
```

---

## Observations

- The neural network achieved **100% training accuracy**.
- All inputs of the AND gate were classified correctly.
- The ReLU activation function improved learning in the hidden layer.
- The Sigmoid activation function produced probability values for binary classification.
- TensorFlow simplified the implementation of model training, evaluation, and prediction.

---

## Conclusion

The Feedforward Neural Network was successfully implemented using TensorFlow and Keras. The network learned the AND gate with perfect accuracy, demonstrating the complete process of building, training, evaluating, and testing a neural network for binary classification tasks.
