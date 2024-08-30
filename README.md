# House2Real: Transform House Outlines Into Realistic Images

## Project Description
House2Real leverages deep learning to transform simple sketches of house outlines into detailed, realistic images. This project is particularly useful for architects, real estate developers, and urban planners. It is developed in a Jupyter Notebook, providing an interactive way to understand the data processing, model building, and output generation.

### Key Features
- **Photorealistic Generation**: Turn architectural outlines into lifelike house images.
- **Interactive Visualization**: Directly interact with the data and model predictions within the Jupyter Notebook.
- **Educational Tool**: Serve as a resource for students and professionals wanting to learn about the application of GANs in real estate and architecture.

## Model Architecture

The House2Real model uses a Generative Adversarial Network (GAN) architecture consisting of two main components:

### Generator
- **Purpose**: Converts outline sketches of houses into realistic images.
- **Structure**: Comprised of several convolutional neural network (CNN) layers, each followed by batch normalization and LeakyReLU activation. The model upscales the input sketch through transposed convolution layers to generate high-resolution images.

### Discriminator
- **Purpose**: Differentiates between the generated images and real images from the training dataset.
- **Structure**: A deeper CNN than the generator, with several convolutional layers that downsample the input to classify it as real or fake. Uses LeakyReLU activation and dropout to prevent overfitting.

The interaction between these two components through adversarial training helps in refining the generated images to look as realistic as possible.

## Dataset

### Overview
Our dataset consists of architectural drawings and corresponding real house images. It has been curated to train the GAN effectively, with the following characteristics:

- **Data Size**: Comprises over 10,000 images, split between sketches and real photos.
- **Variety**: Includes a diverse range of house designs, from modern urban structures to traditional homes.
- **Preprocessing**: All images are resized to a uniform dimension and normalized to aid in model training.

### Sources
[The images are sourced from various public architectural databases and real estate listings to provide a comprehensive learning dataset.
](https://www.kaggle.com/datasets/ramiromep/house-thumbnail)

### Usage
The dataset is split into training and validation sets. The training set is used to train the GAN, while the validation set helps in fine-tuning the model parameters and preventing overfitting.

By detailing the architecture and dataset in your README, potential users and contributors can gain a better understanding of how your model works and the type of data it has been trained on. This information is crucial for anyone looking to replicate the study, contribute to the project, or use the model for their own applications.


## Getting Started

### Prerequisites
Ensure you have Jupyter Notebook or JupyterLab installed, which can be done through Anaconda or directly with pip:
```bash
pip install notebook
```
## Installation
Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/yourusername/House2Real.git
cd House2Real
```

## Output Examples
![Example2](https://github.com/user-attachments/assets/4180cae8-f4a8-462f-ae4d-38dc2849eebb)

![Example2](https://github.com/user-attachments/assets/7181cba4-0611-4e51-93c4-1dd68e12452e)

