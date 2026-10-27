# Fuzzy Hopfield Network for Digit Recognition

## 1. Introduction

This project implements a Fuzzy Hopfield Network to recognize and reconstruct noisy digit patterns. It uses fuzzy logic to handle uncertainty in image pixels and compares its performance with a traditional Hopfield Network.

The project is developed using Python and NumPy without using pre-trained machine learning models.

## 2. Objectives

- To understand the working of Hopfield Neural Networks.
- To implement fuzzy logic in pattern recognition.
- To reconstruct digit patterns affected by noise.
- To compare the performance of fuzzy and traditional Hopfield Networks.
- To evaluate recognition accuracy at different noise levels.

## 3. Technologies Used

- Python 3
- NumPy
- Hopfield Neural Network
- Fuzzy Logic

## 4. Project Description

The system stores five digit patterns: 0, 1, 2, 3, and 5. Each digit is represented using a 7 × 7 grid of pixels.

Noise is added to the stored digit patterns to simulate damaged or unclear images. The network processes the noisy input and attempts to recover the original digit.

Two methods are compared:

1. **Traditional Hopfield Network:** Uses hard thresholding to update neuron states.
2. **Fuzzy Hopfield Network:** Uses fuzzy membership values to handle uncertain pixel information.

The fuzzy system also calculates similarity scores and produces a confidence-based decision.

## 5. Working Methodology

The project follows these steps:

1. Create digit patterns using a 7 × 7 grid.
2. Add random noise to the digit images.
3. Normalize the pixel values.
4. Convert the input into fuzzy membership values.
5. Train the Hopfield Network using the Hebbian learning rule.
6. Reconstruct the noisy patterns using both methods.
7. Compare the reconstructed patterns with the stored digits.
8. Evaluate performance at different noise levels.

## 6. Installation

Make sure Python 3 is installed on your system.

Install the required library:

```bash
python -m pip install numpy
```

## 7. How to Run

Open a terminal in the project directory and execute:

```bash
python fuzzy_hopfield_digits.py
```

The program displays the original digit, noisy input, reconstructed output, predicted digit, confidence score, and performance comparison.

## 8. Expected Output

The program produces:

- Original digit patterns.
- Noisy digit patterns.
- Reconstructed digit patterns.
- Predicted digit and confidence verdict.
- Similarity scores.
- Comparison of traditional and fuzzy Hopfield Network accuracy at different noise levels.

Actual results may vary depending on the patterns, noise settings, and experimental configuration.

## 9. Applications

- Pattern recognition.
- Image restoration.
- Noise removal in simple binary images.
- Associative memory systems.
- Studying fuzzy logic in neural networks.

## 10. Limitations

- The system uses small, manually defined digit patterns.
- It is not designed to recognize real-world handwritten digits.
- Similar patterns may be confused when noise is high.
- The experiment uses synthetic data rather than real image datasets.
- Performance depends on the network configuration and stored patterns.

## 11. Future Improvements

- Add more digit patterns.
- Test different fuzzy membership functions.
- Evaluate additional noise levels.
- Generate accuracy graphs using Matplotlib.
- Test the model on real handwritten digit images.

## 12. Conclusion

This project demonstrates how fuzzy logic can be combined with a Hopfield Network to reconstruct noisy digit patterns. It compares fuzzy and traditional approaches and examines how noise affects their recognition performance.

The project provides a practical introduction to associative memory, fuzzy logic, and neural network-based pattern recognition.
