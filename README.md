# Iranian License Plate Recognition

## Overview

The **Iranian License Plate Recognition** project uses machine learning to identify and read license plate numbers from images of Iranian vehicles. It employs computer vision techniques and a logistic regression model to process license plate images and predict the individual digits and characters specific to Iranian license plates.

## Features

- **Image Processing**: Resizes and converts Iranian license plate images to grayscale.
- **Data Preparation**: Flattens image data and prepares it for machine learning.
- **Model Training**: Trains a logistic regression model on a dataset of Iranian license plate digits and characters.
- **Plate Segmentation**: Segments individual characters from a full Iranian license plate image.
- **Digit Recognition**: Predicts digits and characters using the trained model.
- **Visualization**: Displays processing steps and results using matplotlib.

## Getting Started

To run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/TahaBakhtari/plate-recognition.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd plate-recognition
   ```

3. **Install Dependencies**:
   ```bash
   pip install numpy opencv-python matplotlib scikit-learn
   ```

4. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook plate_recognition.ipynb
   ```

## Dataset

The project uses a custom dataset of Iranian license plate digit and character images stored in numbered folders (1-9). Each folder contains multiple images of the corresponding digit or character.

## Key Components

- Image preprocessing and resizing for Iranian license plates
- Feature extraction through image flattening
- Logistic regression model for digit and character classification
- License plate segmentation algorithm tailored for Iranian plates
- Custom prediction function for individual digits and characters

## Results

The model achieves an accuracy of approximately 91.15% on the test set. It can successfully segment and recognize digits and characters from full Iranian license plate images.

## Iranian License Plate Format

The project is designed to work with the standard Iranian license plate format:
- Two digits
- One letter (in Persian)
- Three digits
- Two digits (usually representing the region code)

Example: 12-365|11 (where | separates the region code)

## Future Improvements

- Implement more advanced deep learning models (e.g., CNNs)
- Enhance plate segmentation for varied lighting conditions
- Expand the dataset for improved accuracy on Iranian plates
- Add real-time recognition capabilities for traffic monitoring
- Incorporate Persian character recognition for the letter in the plate

## Note: 
The number plate photo folders cannot be uploaded on Gainhub due to the large number of them.
Please extract the plates_file.zip file and put folders 1 to 9 in the root of the project itself


## Note: 
This model only learns and predicts numbers and does not have the ability to predict and recognize letters yet !

## License

This project is open-source and available under the MIT License.
