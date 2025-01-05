# Image-Captioning

Image Captioning project made using CNN & LSTM.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Notebooks](#notebooks)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project aims to generate captions for images using a combination of Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) networks. The CNN is used to extract features from the images, and the LSTM is used to generate captions based on these features.

## Features
- Extracts features from images using a pre-trained CNN.
- Generates captions using an LSTM network.
- Supports training on custom datasets.
- Provides evaluation metrics to assess the quality of generated captions.

## Project Structure
Image-Captioning/ 
├── .gitignore\ 
├── app.py\ 
├── Dataset/\ 
│ ├── captions.txt\ 
│ └── Images/\ 
├── test-images/\ 
├── LICENSE\ 
├── models/\ 
│ ├── feature_extractor.keras\ 
│ ├── model.keras\ 
│ └── tokenizer.pkl\ 
├── Notebooks/\ 
│ └── flickr8k-image-captioning-using-cnns-lstm.ipynb\ 
├── README.md\ 
├── requirements.txt\ 
└── venv/\

## Installation

1. Clone the repository:
    ```sh
    git clone <repository-url>
    ```
2. Navigate to the project directory:
    ```sh
    cd Image-Captioning
    ```
3. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
4. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

1. Run the application:
    ```sh
    python app.py
    ```

## Dataset
The project uses the Flickr8k dataset for training and evaluation. You can download the dataset from [here](https://www.kaggle.com/datasets/adityajn105/flickr8k).

## Model Architecture
The model consists of two main components:
1. **CNN (Convolutional Neural Network)**: Used to extract features from images. A pre-trained model like VGG16 or ResNet50 can be used.
2. **LSTM (Long Short-Term Memory)**: Used to generate captions based on the features extracted by the CNN.

## Training
To train the model, follow the steps in the Jupyter notebook:
- flickr8k-image-captioning-using-cnns-lstm.ipynb

## Evaluation
To evaluate the model, you can use the `generate_and_display_caption` function in the [app.py](http://_vscodecontentref_/4) file to generate captions for test images and visually inspect the results.

## Notebooks
Explore the Jupyter notebook for detailed steps and explanations:
- flickr8k-image-captioning-using-cnns-lstm.ipynb

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](http://_vscodecontentref_/5) file for details.