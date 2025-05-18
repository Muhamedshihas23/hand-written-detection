# MNIST Digit Classifier with CNN

This project builds a **Convolutional Neural Network (CNN)** using TensorFlow/Keras to classify handwritten digits from the **MNIST** dataset.

## 🧠 Overview

The model is trained to recognize digits from 0 to 9 using grayscale images of size 28x28 pixels. It leverages CNN layers to automatically extract spatial features and achieves high accuracy on test data.

### Key Features:
- Loads and visualizes MNIST dataset.
- Preprocesses the images (normalization and reshaping).
- Builds a CNN with two convolutional blocks.
- Trains the model using `categorical_crossentropy` loss and `adam` optimizer.
- Evaluates performance and visualizes predictions.
- Saves the model in multiple formats (`.h5`, `.keras`, and TensorFlow SavedModel).

## 🧪 Dataset

- **MNIST**: 70,000 handwritten digit images (60,000 for training, 10,000 for testing).
- Automatically downloaded using `tensorflow.keras.datasets`.

## 🛠️ Requirements

Install the following Python packages:

```bash
pip install tensorflow matplotlib numpy
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. Run the script:
   ```bash
   python detection.py
   ```

3. After training, you will see:
   - Sample predictions on test data.
   - Saved models:
     - `mnist_digit_classifier.h5`
     - `mnist_digit_classifier.keras`
     - `mnist_model/` folder (TensorFlow SavedModel format)

## 📊 Model Summary

```
Conv2D → MaxPooling2D → Conv2D → MaxPooling2D → Flatten → Dense(128) → Dropout(0.3) → Dense(10)
```

## 📈 Accuracy

The trained model achieves ~98–99% accuracy on test data depending on training conditions.

## 📁 Outputs

- `mnist_digit_classifier.h5`
- `mnist_digit_classifier.keras`
- `mnist_model/` (TensorFlow SavedModel format)

## 📸 Sample Output

Images with predicted digit labels are displayed after training.

---

## 🔖 License

This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Contributions

Feel free to fork the repo, make changes, and submit a pull request.
