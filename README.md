

---

# Loan Eligibility Predictor

## Overview

This project predicts loan eligibility for applicants based on personal, financial, and property-related information. It utilizes machine learning models, including Random Forest and Neural Networks, and offers a user-friendly Streamlit web interface for real-time predictions.

## Table of Contents

- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
  - [Training the Model](#training-the-model)
  - [Testing the Model](#testing-the-model)
  - [Running the Web Application](#running-the-web-application)
- [File Descriptions](#file-descriptions)
- [License](#license)

## Project Structure


```bash
LoanEligibilityPredictor/
├── assets/                 # Contains images and other assets
├── dataset/                # Contains the dataset files
├── app.py                  # Streamlit web application
├── eda.ipynb               # Exploratory Data Analysis notebook
├── LoanerNN.ipynb          # Neural Network model notebook
├── LoanerRFC.ipynb         # Random Forest Classifier notebook
├── nn.py                   # Neural Network model script
├── utils.py                # Utility functions
├── requirements.txt        # Python dependencies
├── environment.yml         # Conda environment configuration
├── README.md               # Project documentation
└── LICENSE                 # License information
```


## Installation

### Using pip


```bash
# Clone the repository
git clone https://github.com/SamarthPyati/LoanEligibilityPredictor.git
cd LoanEligibilityPredictor

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```


### Using Conda


```bash
# Clone the repository
git clone https://github.com/SamarthPyati/LoanEligibilityPredictor.git
cd LoanEligibilityPredictor

# Create and activate the Conda environment
conda env create -f environment.yml
conda activate loan-eligibility
```


## Usage

### Training the Model

To train the model using the Random Forest Classifier:


```bash
# Run the training notebook
jupyter notebook LoanerRFC.ipynb
```


Alternatively, for the Neural Network model:


```bash
# Run the training notebook
jupyter notebook LoanerNN.ipynb
```


These notebooks will guide you through the training process, including data preprocessing, model training, and evaluation.

### Testing the Model

Testing is integrated within the training notebooks. After training, the notebooks include evaluation metrics such as accuracy, precision, recall, and ROC-AUC scores to assess model performance.

### Running the Web Application

To launch the Streamlit web application for real-time loan eligibility predictions:


```bash
streamlit run app.py
```


This will open a web interface where you can input applicant details and receive eligibility predictions.

## File Descriptions

- **`app.py`**: Main Streamlit application script that provides a web interface for users to input data and receive predictions.
- **`eda.ipynb`**: Notebook for Exploratory Data Analysis, including data visualization and initial insights.
- **`LoanerRFC.ipynb`**: Notebook detailing the training process using the Random Forest Classifier.
- **`LoanerNN.ipynb`**: Notebook detailing the training process using a Neural Network model.
- **`nn.py`**: Python script containing the implementation of the Neural Network model.
- **`utils.py`**: Contains utility functions used across the project, such as data preprocessing functions.
- **`requirements.txt`**: Lists all Python dependencies required to run the project.
- **`environment.yml`**: Conda environment configuration file listing dependencies and environment settings.
- **`assets/`**: Directory containing images and other assets used in the project.
- **`dataset/`**: Directory containing the dataset files used for training and testing.

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).

---

