# 📰 Fake News Detection using Neural Networks

This repository contains a Deep Learning project designed to classify news headlines as either **Real** or **Fake** using a Feedforward Neural Network.

## 🔗 Dataset
The model was trained using the **WELFake Dataset** available on Kaggle.
* **Dataset Link:** [WELFake Dataset on Kaggle](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification)
* **Description:** 72,134 news articles with labels (0 for Real, 1 for Fake).

## 🧠 Model Architecture
The model is a Sequential Feedforward Neural Network built with TensorFlow/Keras:

| Layer | Type | Configuration | Activation |
| :--- | :--- | :--- | :--- |
| **Input** | Dense | 5,000 Features (TF-IDF) | - |
| **Hidden 1** | Dense | 128 Neurons | ReLU |
| **Hidden 2** | Dense | 64 Neurons | ReLU |
| **Output** | Dense | 1 Neuron | Sigmoid |

### Hyperparameters:
* **Optimizer:** Adam
* **Loss Function:** Binary Crossentropy
* **Epochs:** 10
* **Batch Size:** 32

## 📈 Performance Summary
* **Test Accuracy:** ~93.7%
* **Key Insight:** During training, I observed that the model reached near 100% training accuracy very quickly, while the validation loss began to rise after the 2nd epoch. This indicates **overfitting**, suggesting that for future improvements, regularization techniques like *Dropout* or *Early Stopping* should be implemented.

## 🛠️ Installation & Usage
1. Clone this repository.
2. Download the dataset from Kaggle and place it in the project folder.
3. Open the `.ipynb` notebook in Google Colab or Jupyter Notebook.
4. Run all cells to preprocess data, train the model, and see predictions.
