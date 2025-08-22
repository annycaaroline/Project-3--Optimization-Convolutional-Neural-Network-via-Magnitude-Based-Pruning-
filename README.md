This project explores deep learning  and pruning techniques for skin lesions using the HAM10000 dataset. The focus is on training convolutional neural networks (CNNs), applying model pruning for compression, and evaluating performance. The entire workflow is implemented in the EDA.ipynb and Training_Pruning_Evaluation.ipynb notebook.

## Table of Contents
   1. Features
   2. Prerequisites
   3. Installation and Setup
   4. License


## Features
- Data processing and augmentation with TensorFlow/Keras.
- Convolutional neural network (CNN) with TensorFlow/Keras.
- Pruning using tensorflow_model_optimization.
- Evaluation metrics including accuracy and loss
- Support for saving and loading trained models.


## Prerequisites
Ensure you have the following installed before running the code:
- Python 3.7 or higher
- TensorFlow 2.13.0
- NumPy 1.26.4
- Pandas
- TFMOT: 0.7.3
- scikit-learn
- [HAM10000 Dataset](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)

or

https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000/code


## Installation and Setup
1. **Install Kaggle API and upload your Kaggle token**:

   ```python
   !pip install kaggle --quiet

   from google.colab import files
   files.upload()  # Upload kaggle.json

Move the Kaggle token and set permissions:

   !mkdir -p ~/.kaggle
   !mv kaggle.json ~/.kaggle/
   !chmod 600 ~/.kaggle/kaggle.json

Download dataset:
!kaggle datasets download -d kmader/skin-cancer-mnist-ham10000 -p /content --unzip

   
2. Install the dependencies:

   !pip install kaggle --quiet
   !pip install -q codecarbon
   !pip install GPUtil --quiet

## License

[MIT License](LICENSE)
This project is licensed under the MIT License - see the LICENSE file for more details.
