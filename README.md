# 📊 Project: Plant Disease Classification with VGG19

A machine learning project to classify plant diseases using images of tomato plants. The project employs transfer learning with the VGG19 model, data augmentation, and fine-tuning to improve accuracy.

---

## 📁 Dataset Preparation

- The dataset was sourced from Kaggle's **New Plant Diseases Dataset**.
- The dataset contains images of various plant diseases, with a specific focus on tomato plant diseases.
- Steps taken:
  - Downloaded the dataset using Kaggle API.
  - Unzipped and extracted the data into training and validation directories.
  - Filtered out relevant tomato plant diseases for classification.

---

## 🔍 Feature Engineering

- Applied data preprocessing techniques to handle the images:
  - **Rescaling**: Image pixel values were rescaled to the range [0, 1].
  - **Data Augmentation**: Techniques like random flips, rotations, zoom, and contrast adjustments were applied to increase diversity in the training data.

---

## 🛠️ Model Implementation

### Model Architecture:
- **VGG19 Model** (pre-trained on ImageNet) was used as the base model for transfer learning.
- The last layers of the VGG19 model were frozen, and the top layers were added for fine-tuning:
  - **Fully Connected Layers**: Dense layers with ReLU activation functions.
  - **Batch Normalization**: To improve model stability.
  - **Dropout Layers**: To prevent overfitting.

### Optimizer and Loss Function:
- **Optimizer**: Adam with a learning rate of `1e-5`.
- **Loss Function**: Categorical Cross-Entropy for multi-class classification.

### Callbacks:
- **Early Stopping**: To prevent overfitting and stop training when validation loss doesn't improve.

---

## ⚙️ Hyperparameter Tuning

- Hyperparameters such as learning rate, batch size, and dropout rate were adjusted to improve model performance.
- Fine-tuned the VGG19 model by unfreezing the last few layers to improve classification accuracy for tomato plant diseases.

---

## 📊 Model Evaluation

- **Metrics**:
  - Accuracy
  - Loss
  - Validation Accuracy
  - Validation Loss
- **Validation Results**: 
  - **Validation Loss**: X.XX
  - **Validation Accuracy**: X.XX%

---

## 🤖 Predictions and Inference

- A sample image of a tomato plant disease was tested on the trained model.
- The model predicted the class of the disease along with the associated probability.

---

## 📄 Documentation

This project includes:
- **Jupyter Notebook** for running the model and predictions.
- Detailed explanation of data preprocessing, model architecture, training process, and evaluation.

---

## 🙌 Acknowledgments

- **Kaggle** for providing the dataset.
- **TensorFlow** and **Keras** for deep learning tools.
- **Matplotlib** for data visualization.

---

## 📬 Contact

For any questions or suggestions, feel free to reach out:

- **Name**: G. Kamesh
- **Email**: kamesh743243@gmail.com
