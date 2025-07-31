# AI 2025 PyTorch Projects

This repository serves as a learning platform and reference implementation for various machine learning tasks using PyTorch. Each project is self-contained with its own implementation, documentation, and results, making it easy to explore different ML concepts and techniques.

---

## 📈 Project Status

| Project | Status | Description |
|---------|--------|-------------|
| [Project 1: Rice Classification](Project1/) | ✅ Complete | Binary classification of rice types |
| [Project 2: Animal Faces Image Classification](Project2/) | ✅ Complete | Image classification of animal faces (98.86% accuracy) |
| [Project 3: Bean Leaf Classification using Transfer Learning](Project3/) | ✅ Complete | Multi-class classification of bean leaf lesions using transfer learning  |

---

## 📚 Requirements

- Python 3.8+
- PyTorch
- Jupyter Notebook
- Other dependencies as listed in `requirements.txt` and project-specific READMEs

---

## 📁 Directory Structure

```
Projects_Pytorch/
├── Project1/
│   ├── RiceClassification.ipynb
│   └── README.md
├── Project2/
│   ├── AnimalFacesClassification.ipynb
│   └── README.md
├── Project3/
│   ├── BeanLeafclassificationusingTransferLearning.ipynb
│   └── README.md
├── requirements.txt
└── README.md
```

---

## 🚀 Getting Started

1. **Clone the repository**
    ```
    git clone https://github.com/yourusername/Projects_Pytorch.git
    cd Projects_Pytorch
    ```

2. **Install dependencies**
    ```
    pip install -r requirements.txt
    ```

3. **Download datasets**
   - Follow instructions in each project folder's README to download and place datasets.

4. **Run the notebooks**
    ```
    jupyter notebook
    ```
   - Open the desired project notebook and follow the steps inside.

---

## 📝 Project Highlights

### Project 1: Rice Classification
- Neural network classifier with PyTorch
- 18,185 rice grain samples with 11 morphological features
- Achieves ~95% classification accuracy
- Complete data analysis and visualization pipeline

### Project 2: Animal Faces Image Classification
- Multi-class classification of animal faces.
- Achieved **98.86% accuracy**.
- Visualization of predictions and training curves.

### Project 3: Bean Leaf Classification using Transfer Learning
- Multi-class classification of bean leaf lesions (healthy, angular_leaf_spot, bean_rust).
- Utilizes transfer learning with pretrained CNNs (e.g., ResNet, VGG).
- Achieved **87.74% accuracy** on the validation set.
- Includes data augmentation, model evaluation, and result visualization.

---

## 🎯 Project Goals

This repository aims to:

1. **Demonstrate PyTorch Best Practices**: Clean, well-documented implementations
2. **Cover Diverse ML Tasks**: Classification, regression, computer vision, NLP, etc.
3. **Provide Learning Resources**: Educational projects with detailed explanations
4. **Show Real-world Applications**: Practical implementations with real datasets
5. **Maintain Code Quality**: Consistent structure and documentation across projects

## 📚 References

- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- See individual project READMEs for dataset links and more details.

---

## 🤝 Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements or new projects.

---

## 📄 License

This repository is licensed under the MIT License.

---