# Skin Disease Identification using Deep Learning

## Overview

In the realm of medical diagnostics, precision and efficiency are paramount, especially in dermatology where visual assessment plays a crucial role. This project leverages the power of Deep Learning to enhance the accuracy of skin disease classification, addressing the subtle distinctions between various skin conditions. By employing advanced convolutional neural networks (CNNs), specifically pre-trained models like DenseNet, VGG, and ResNet, we aim to automate the analysis of dermatological images, providing a robust tool to aid healthcare professionals.

The integration of Gradient-weighted Class Activation Mapping (Grad-CAM) offers additional insights by highlighting key areas in images that influence the model’s predictions, thereby adding a layer of interpretability to the AI’s decision-making process. Through rigorous model training and validation, coupled with extensive hyperparameter optimization using Optuna, this project aspires to bridge the gap between clinical dermatology and artificial intelligence. Our goal is to transform diagnostic procedures by delivering swift, accurate, and interpretable results.

## File Purpose Explanation

- **download_images.ipynb**: Notebook used to download the Fitzpatrick17k images into the 'images' folder.
- **fitzpatrick17k_csv**: Original provided dataset.
- **fitzpatrick17k_processed.csv**: Processed dataset using the 'download_images' notebook. This CSV contains the local paths to read the images in the source code notebooks.
- **source_code_main.ipynb**: Main notebook containing the source code for the development of the project.
- **source_code_models_with_hair_removal.ipynb**: Notebook demonstrating that models using images with removed body hair performed worse.

## Technologies Used

- **Deep Learning Frameworks**: TensorFlow, Keras, PyTorch
- **Pre-trained Models**: DenseNet, VGG, ResNet
- **Hyperparameter Optimization**: Optuna
- **Visualization Tools**: Matplotlib, Grad-CAM
- **Data Processing**: Pandas, NumPy
- **Notebook Environment**: Jupyter Notebook

## Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.x
- Jupyter Notebook
- TensorFlow
- Keras
- PyTorch
- Pandas
- NumPy
- Matplotlib
- Optuna

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/Muhammadurasheed/notchAI-deep-learnig-model.git
    ```
2. Navigate to the project directory:
    ```sh
    cd skin-disease-classification
    ```
3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

### Usage

1. **Download Images**:
    - Open and run the `download_images.ipynb` notebook to download the Fitzpatrick17k images into the 'images' folder.
  
2. **Process Dataset**:
    - Ensure the `fitzpatrick17k_processed.csv` is generated by running the `download_images.ipynb` notebook.
  
3. **Run Main Code**:
    - Open and run the `source_code_main.ipynb` notebook to execute the main project code.

4. **Evaluate Models with Hair Removal**:
    - Open and run the `source_code_models_with_hair_removal.ipynb` notebook to see the performance impact of removing body hair from images.

### Results

- The project demonstrates significant improvements in the accuracy of skin disease classification through the use of advanced CNN architectures and hyperparameter optimization.
- Grad-CAM visualizations provide interpretability, highlighting the key areas in images that influence the model's predictions.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
