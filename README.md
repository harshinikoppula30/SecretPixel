# SecretPixel — Deep Learning Based Image Steganography

An image steganography project using deep learning to hide and recover secret images within cover images.

## Technologies Used

* Python
* TensorFlow
* Keras
* Convolutional Neural Networks (CNN)
* NumPy
* Matplotlib
* Google Colab
* Gradio

## About the Project

SecretPixel uses a deep learning model to hide a secret image inside a cover image. The model produces an encoded image that looks similar to the original cover image. A decoder network is then used to recover the hidden secret image.

## How It Works

```text
Secret Image + Cover Image
           ↓
        Encoder
           ↓
    Encoded Cover Image
           ↓
        Decoder
           ↓
    Recovered Secret Image
```

## Model

The project uses convolutional neural networks for:

* Preparing features from the secret image
* Hiding the secret image inside the cover image
* Recovering the secret image from the encoded image

The model is trained using image reconstruction losses based on the difference between the original and reconstructed images.

## Dataset

The project uses the **Tiny ImageNet** dataset for training and testing.

## Project Notebook

The complete implementation was developed using **Google Colab**.

The project code is available in the `.ipynb` notebook included in this repository.

## Gradio Interface

A **Gradio interface** is included to allow users to provide a cover image and a secret image and generate:

* Encoded Cover Image
* Recovered Secret Image

## Output

The project generates:

* Original Cover Image
* Secret Image
* Encoded Cover Image
* Recovered Secret Image
