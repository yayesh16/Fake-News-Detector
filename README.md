# Fake News Detection using Neural Networks

This project uses a Feedforward Neural Network to classify news headlines as **Real** or **Fake**.

## 📊 Model Architecture
- **Input:** TF-IDF Vectorization (5,000 features)
- **Hidden Layers:** 2 Dense layers (128 & 64 neurons)
- **Activation:** ReLU for hidden layers, Sigmoid for output
- **Optimizer:** Adam
- **Epochs:** 10 (Early stopping recommended at Epoch 2)

## 📈 Performance
- **Accuracy:** ~93.7%
- **Observation:** The model showed signs of overfitting after the 2nd epoch, as validation loss began to increase while training accuracy reached 100%.

## 🚀 How to use
1. Open the `.ipynb` file in Google Colab.
2. Upload the `WELFake_Dataset.csv`.
3. Run all cells to train and test.
