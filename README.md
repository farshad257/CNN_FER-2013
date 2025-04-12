
# CNN Image Classification with EfficientNetB4

This project presents an image classification pipeline using a convolutional neural network (CNN) based on EfficientNetB4 architecture. The model is designed to handle a custom image dataset, leveraging advanced data augmentation and regularization techniques to enhance performance and prevent overfitting.

## 🏢 Model Architecture

- **Base Model**: EfficientNetB4 (pre-trained on ImageNet)
- **Top Layers**: Custom classification head
- **Regularization**: L1, L2 weight penalties
- **Augmentation**: Random flip, rotation, zoom
- **Training Strategy**:
  - EarlyStopping to avoid overfitting
  - ModelCheckpoint to save the best model

## 📁 Dataset
> <a href= 'https://www.kaggle.com/datasets/farshadtofighi/fer-2013'>***FER_2013***</a>
 - **Structure**:
  ```
  /train
    /class_1
      image1.jpg
      image2.jpg
    /class_2
      ...
  /test
    /class_1
      ...
    /class_2
      ...
  ```
- Images are automatically loaded and labeled from directory structure using TensorFlow's `ImageDataGenerator`.

## ⚙️ Dependencies

- Python 3.x
- TensorFlow 2.x
- NumPy, Pandas, Matplotlib, Seaborn
- scikit-learn

## 📊 Evaluation

The model's performance is assessed using:
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- Accuracy metrics over training epochs

## 📈 Visualization

- Loss and Accuracy plots
- Confusion matrix heatmap
- Example predictions

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Place your dataset inside the `train` and `test` directories.

4. Run the notebook:
   ```bash
   jupyter notebook CNN_Model.ipynb
   ```

## 📌 Notes

- Make sure the dataset is well-organized as described.
- You can easily swap EfficientNetB4 with other architectures using Keras Applications.

## 📧 Contact

For questions or suggestions, feel free to open an issue or contact the maintainer.

---

> **Author**: <span onclick="navigator.clipboard.writeText('farshadtfgh@gmail.com')" style="cursor:pointer; color:blue; text-decoration:underline;">**Farshad Tofighi**</span> (*farshad257*)  
> **License**: MIT

> **Email**: [farshadtfgh@gamil.com](mailto:farshadtfgh@gamil.com)
