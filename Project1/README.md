# Rice Type Classification Project

A binary classification project for identifying different types of rice based on morphological characteristics extracted from rice grain images using PyTorch.

## 📊 Project Overview

This project implements a neural network classifier to distinguish between two types of rice based on morphological features extracted from rice grain images. The model analyzes various geometric and shape characteristics to accurately classify rice types.

### Dataset Information
- **Source**: Rice grain morphological measurements dataset
- **Samples**: 18,185 rice grain samples
- **Classes**: 2 rice types (binary classification)
- **Features**: 11 morphological characteristics

### Key Features
- **Area**: Total area of the rice grain
- **MajorAxisLength**: Length of the major axis
- **MinorAxisLength**: Length of the minor axis
- **Eccentricity**: Measure of how much the grain deviates from being circular
- **ConvexArea**: Area of the convex hull
- **EquivDiameter**: Diameter of a circle with the same area
- **Extent**: Ratio of the grain area to the bounding box area
- **Perimeter**: Perimeter of the rice grain
- **Roundness**: Measure of how round the grain is
- **AspectRatio**: Ratio of major axis to minor axis
- **Class**: Target variable (rice type)

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- PyTorch
- scikit-learn
- pandas, numpy
- matplotlib, seaborn
- jupyter

### Installation
```bash
# Navigate to the project directory
cd Project1/

# Install dependencies (if not already installed)
pip install torch torchvision
pip install scikit-learn pandas numpy
pip install matplotlib seaborn jupyter
```

### Running the Project
```bash
# Start Jupyter notebook
jupyter notebook TabularDataClassification.ipynb
```

## 📁 Project Structure

```
Project1/
├── README.md                           # This file
├── TabularDataClassification.ipynb     # Main analysis notebook
└── ../Datasets/riceClassification.csv  # Dataset file
```

## 🔬 Technical Implementation

### Data Preprocessing
1. **Data Loading**: Import rice classification dataset
2. **Exploratory Analysis**: Statistical analysis and visualization
3. **Feature Scaling**: Standardization of numerical features
4. **Train/Test Split**: 80/20 split for model evaluation

### Model Architecture
- **Input Layer**: 10 features (excluding target variable)
- **Hidden Layers**: Fully connected neural network
- **Activation**: ReLU for hidden layers, Sigmoid for output
- **Loss Function**: Binary Cross Entropy Loss
- **Optimizer**: Adam optimizer

### Training Process
- **Epochs**: Configurable training iterations
- **Batch Size**: Mini-batch gradient descent
- **Validation**: Performance monitoring during training
- **Early Stopping**: Prevent overfitting

### Evaluation Metrics
- **Accuracy**: Overall classification accuracy
- **Precision**: True positive rate
- **Recall**: Sensitivity
- **F1-Score**: Harmonic mean of precision and recall
- **Confusion Matrix**: Detailed classification results

## 📈 Results & Analysis

### Model Performance
- **Training Accuracy**: ~95%+
- **Test Accuracy**: ~94%+
- **Cross-validation**: Robust performance across folds

### Key Findings
1. **Feature Importance**: Area and perimeter are most predictive
2. **Model Convergence**: Stable training with minimal overfitting
3. **Classification Quality**: High precision and recall for both classes

### Visualizations
- Feature distributions and correlations
- Training/validation loss curves
- Confusion matrix heatmap
- Feature importance analysis

## 🛠️ Usage Examples

### Basic Usage
```python
# Load the notebook and run all cells
# The notebook contains complete analysis from data loading to model evaluation
```

### Customization
- Modify hyperparameters in the model definition
- Adjust training parameters (epochs, learning rate)
- Change feature preprocessing methods
- Experiment with different architectures

## 📊 Dataset Details

### Data Source
The dataset contains morphological measurements of rice grains, including:
- Geometric properties (area, perimeter, axis lengths)
- Shape characteristics (roundness, eccentricity)
- Derived features (aspect ratio, extent)

### Data Quality
- **Missing Values**: None
- **Duplicates**: Handled during preprocessing
- **Outliers**: Analyzed and treated appropriately
- **Class Balance**: Well-balanced dataset

## 🔧 Dependencies

### Core Libraries
```python
torch                    # PyTorch for deep learning
scikit-learn            # Machine learning utilities
pandas                  # Data manipulation
numpy                   # Numerical computing
matplotlib              # Basic plotting
seaborn                 # Statistical visualization
jupyter                 # Interactive notebooks
```

### Optional Libraries
```python
torchsummary            # Model architecture visualization
kagglehub              # Dataset access (if needed)
```

## 🎯 Project Goals

1. **Binary Classification**: Accurately classify rice types
2. **Feature Analysis**: Understand important morphological features
3. **Model Optimization**: Achieve high classification accuracy
4. **Reproducibility**: Clear, documented implementation

## 📝 Notes

- The notebook contains complete analysis with detailed comments
- All visualizations are included for comprehensive understanding
- Model architecture can be easily modified for experimentation
- Results are reproducible with the provided code

## 🤝 Contributing

Feel free to:
- Improve the model architecture
- Add new evaluation metrics
- Enhance visualizations
- Optimize hyperparameters
- Add new preprocessing techniques

## 📞 Support

For questions or issues:
- Check the notebook comments for detailed explanations
- Review the data preprocessing steps
- Examine the model architecture section
- Contact the project maintainer

---

**Last Updated**: [07/20/2025]
**Status**: ✅ Complete and Functional 