# DCGAN Image Generator - MNIST Dataset

This project implements a **Deep Convolutional Generative Adversarial Network (DCGAN)** to generate images of handwritten digits using the **MNIST dataset**. The generator learns to create realistic images of digits, while the discriminator distinguishes between real and generated images.

## Project Overview

The **DCGAN** architecture consists of two neural networks:
1. **Generator**: Creates images from random noise (latent vectors).
2. **Discriminator**: Attempts to distinguish between real MNIST images and fake images produced by the generator.

This implementation is trained using the MNIST dataset, which contains 28x28 grayscale images of handwritten digits (0-9).

## Features

- **DCGAN Architecture**: Uses deep convolutional layers to both generate and evaluate images.
- **Training on MNIST Dataset**: Uses the MNIST dataset of handwritten digits for training and evaluation.
- **Image Generation**: The trained model can generate new, realistic images resembling handwritten digits.

## Requirements

- Python 3.x
- TensorFlow 2.x
- Keras
- NumPy
- Matplotlib

You can install the dependencies using the following:

```bash
pip install -r requirements.txt
```

## How to Use

### 1. Clone the repository

```bash
git clone https://github.com/alihassanml/DCGAN-Image-Generate.git
cd DCGAN-Image-Generate
```

### 2. Train the Model

To train the DCGAN model on the MNIST dataset, simply run the following:

```bash
python train.py
```

This will load the MNIST dataset, train the DCGAN model, and save the generated images at each epoch.

### 3. Generate Images

After training, you can generate new images using the trained generator. To do this, run:

```bash
python generate.py
```

This will generate and display new images of handwritten digits.

## Project Structure

```
DCGAN-Image-Generate/
│
├── data/                # MNIST dataset
├── images/              # Generated images
├── models/              # Saved models
├── train.py             # Script to train the DCGAN model
├── generate.py          # Script to generate new images using the trained model
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Results

The trained model will generate images resembling handwritten digits, similar to the MNIST dataset.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
