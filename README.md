# FinalProject

## Project Overview:
This project trains a deep learning model to estimate the number of spermatozoa cells in three categories (normal, clustered, and pinhead) from microscopy images. The model learns to predict total counts directly from the image using a convolutional encoder. Two versions of the model are tested, a base model using a U-Net-like encoder and a slightly more advanced version that adds Squeeze-and-Excitation (SE) blocks to improve performance.

## How to run:
To run this, first use the 2nd_cnn_env.yml to set up the enviroment. Then inside DLproject.ipynb, you need to edit the file paths to match your machine. These include PROJECT_ROOT, CSV_PATH, and the Train/Test folders. Then run DLproject.ipynb and it will 
- Load the dataset
- Train both models
- Save the best versions as best_model.pth and best_se_model.pth
- Plot the predictions versus the true counts
- Evaluate both models on a the held-out test set

The dataset used was from the VISEM Tracking dataset and is publically available.
