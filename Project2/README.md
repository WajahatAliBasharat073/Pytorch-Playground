# Project 2: Image Classification with PyTorch

## Overview
This project demonstrates image classification using PyTorch. The goal is to classify images of animals (cats, dogs, wild animals) using a convolutional neural network (CNN). The project is structured as a Jupyter notebook for easy experimentation and visualization.

## Dataset
- **Source**: `../Datasets/AnimalFaces/`
- **Classes**: Cat, Dog, Wild
- **Structure**:
  - `train/` and `val/` folders, each containing subfolders for each class
  - Example: `train/cat/`, `train/dog/`, `train/wild/`
- **Sample Image**: `cat.jpg` (provided for quick testing)

## Usage
1. Open `imageClassification.ipynb` in Jupyter Notebook or VSCode.
2. Follow the notebook cells to:
   - Load and preprocess the dataset
   - Define and train a CNN model
   - Evaluate model performance
   - Visualize predictions

## Requirements
- Python 3.8+
- PyTorch
- torchvision
- matplotlib, numpy, pandas

Install dependencies from the root directory:
```bash
pip install -r requirements.txt
```

## Results
- The notebook demonstrates training and evaluation of a CNN on the AnimalFaces dataset.
- Includes sample visualizations and accuracy metrics.

## Files
- `imageClassification.ipynb`: Main notebook for the project
- `cat.jpg`: Example image for quick testing

## References
- [PyTorch Documentation](https://pytorch.org/docs/stable/index.html)
- [Animal Faces Dataset](https://www.kaggle.com/datasets/alessiocorrado99/animal-faces)

---

**Note:** Update the dataset path in the notebook if your folder structure differs. 