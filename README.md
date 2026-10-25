# CIFAR-10 Image Classification

A convolutional neural network that classifies 32x32 color images into 10 categories (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck), trained on the CIFAR-10 dataset.

## Results

| Metric | Value |
|---|---|
| Test accuracy | [XX.X%] |
| Training epochs | [N] |
| Framework | [TensorFlow/Keras or PyTorch] |

## Model Architecture

- [e.g. 3 convolutional blocks (Conv2D + BatchNorm + MaxPool)]
- [e.g. Dropout for regularization]
- [e.g. Dense layer + softmax output with 10 classes]
- [Data augmentation, if you used it: flips, shifts, etc.]

## Dataset

[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html): 60,000 images (50,000 train, 10,000 test) across 10 classes. It is not included in this repo and downloads automatically when you run the code.

## Project Structure

```
.
├── [notebook_or_script].ipynb   # training and evaluation
├── [model_file].keras           # saved trained model
├── requirements.txt
└── README.md
```

## Setup

```bash
git clone https://github.com/SaFal252/cifar10-image-classification.git
cd cifar10-image-classification
python -m venv venv
venv\Scripts\activate        # Mac/Linux: source venv/bin/activate
pip install -r requirements.txt
```

## Usage

Train the model:
```bash
python [train.py]
```

Load the saved model and predict:
```python
from tensorflow.keras.models import load_model

model = load_model("[model_file].keras")
# preprocess your image to 32x32, scale to [0, 1], then:
# prediction = model.predict(image)
```

## Future Improvements

- Try transfer learning (e.g. ResNet or MobileNet)
- Deploy as a web app (Streamlit or Django)
- Add a confusion matrix and per-class accuracy

## Author

**Safal Shrestha**
[GitHub](https://github.com/SaFal252) | [LinkedIn](https://linkedin.com/in/safal-shrestha01)