# Rice Type Classification Project

A machine learning project for classifying different types of rice using PyTorch and deep learning techniques. This project analyzes rice grain characteristics to predict rice varieties based on morphological features.

## 📋 Project Overview

This project implements a neural network classifier to identify different types of rice based on various morphological characteristics extracted from rice grain images. The dataset contains measurements of rice grains including area, axis lengths, eccentricity, and other geometric properties.

### Dataset Features

The dataset includes the following features for each rice grain:
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

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. **Clone or download the project**
   ```bash
   # If using git
   git clone <repository-url>
   cd Projects_Pytorch
   ```

2. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. **Install required dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 📁 Project Structure

```
Projects_Pytorch/
├── Datasets/
│   └── riceClassification.csv          # Rice classification dataset
├── Project1/
│   └── TabularDataClassification.ipynb # Main Jupyter notebook
├── requirements.txt                    # Python dependencies
├── README.md                          # This file
└── venv/                              # Virtual environment (created locally)
```

## 🎯 Usage

### Running the Jupyter Notebook

1. **Start Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

2. **Open the notebook**
   - Navigate to `Project1/TabularDataClassification.ipynb`
   - Run cells sequentially to execute the analysis

### Data Loading Options

The notebook provides two methods for loading the dataset:

#### Option 1: Local Dataset
```python
# Load from local file
df = pd.read_csv('Datasets/riceClassification.csv')
```

#### Option 2: Kaggle Dataset (Recommended)
```python
# Install kagglehub if not already installed
# pip install "kagglehub[pandas-datasets]"

import kagglehub
from kagglehub import KaggleDatasetAdapter

# Load dataset from Kaggle
df = kagglehub.load_dataset(
    KaggleDatasetAdapter.PANDAS,
    "mssmartypants/rice-type-classification",
    "rice_classification_kaggle.csv"
)
```

## 🔧 Key Libraries Used

- **PyTorch**: Deep learning framework for neural network implementation
- **scikit-learn**: Machine learning utilities for preprocessing and evaluation
- **pandas**: Data manipulation and analysis
- **numpy**: Numerical computing
- **matplotlib & seaborn**: Data visualization
- **kagglehub**: Dataset access from Kaggle

## 📊 Analysis Workflow

The notebook follows this general workflow:

1. **Data Loading**: Import the rice classification dataset
2. **Data Exploration**: Analyze dataset structure and statistics
3. **Data Preprocessing**: 
   - Handle missing values
   - Remove duplicates
   - Drop unnecessary columns (like 'id')
   - Feature scaling and encoding
4. **Model Development**: 
   - Design neural network architecture
   - Train the model
   - Evaluate performance
5. **Results Analysis**: 
   - Generate classification reports
   - Create confusion matrices
   - Visualize results

## 🤝 Contributing

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Dataset source: [Rice Type Classification Dataset](https://www.kaggle.com/datasets/mssmartypants/rice-type-classification)
- Built with PyTorch and scikit-learn
- Visualization tools: matplotlib and seaborn

## 📞 Contact

For questions or support, please open an issue in the repository or contact the project maintainer.

---

**Note**: Make sure to activate your virtual environment before running the notebook to ensure all dependencies are available.
