# Bean Leaf Classification using Transfer Learning

This project focuses on classifying bean leaf lesions into three categories—__healthy__, __angular_leaf_spot__, and __bean_rust__—using transfer learning with PyTorch. The goal is to assist in early detection of bean plant diseases through automated image analysis.

---

## 📂 Dataset

- **Source:** [Kaggle - Bean Leaf Lesions Classification](https://www.kaggle.com/datasets/marquis03/bean-leaf-lesions-classification)
- **Images:** 1034 for training, 133 for validation
- __Classes:__ healthy, angular_leaf_spot, bean_rust
- **Format:** Images with CSV files for labels

---

## 🛠️ Approach

- Utilizes transfer learning with pretrained CNNs (e.g., ResNet, VGG)
- Custom PyTorch `Dataset` class for image loading and preprocessing
- Data augmentation and normalization
- Model training, validation, and performance visualization

---

## 📊 Results

- **Achieved Accuracy:** 87.74% on the validation set
- Includes visualizations of predictions and training curves

---

## 📁 Directory Structure

```ini
Project3/
├── BeanLeafclassificationusingTransferLearning.ipynb
├── README.md

```

---

## 🚀 Usage

1. **Install dependencies:**

```sh
pip install -r ../requirements.txt

```

2. **Download the dataset** and place it in `Datasets/Bean Leaf Classification/` as described in the notebook.

3. **Run the notebook:**

```sh
jupyter notebook BeanLeafclassificationusingTransferLearning.ipynb

```

---

## 📚 References

- [Kaggle Dataset](https://www.kaggle.com/datasets/marquis03/bean-leaf-lesions-classification)
- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)