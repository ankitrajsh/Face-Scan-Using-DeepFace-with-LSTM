# Face Scan Project

## Overview

The Face Scan Project is designed to generate consistent face embeddings for a given individual across multiple images. By leveraging state-of-the-art models such as RetinaFace for face detection and DeepFace's FaceNet512 for embedding generation, this project ensures that each image of the same person yields identical 128-dimensional vectors. The embeddings are further refined using an LSTM (Long Short-Term Memory) model to achieve high precision in face recognition tasks.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Pipeline Overview](#pipeline-overview)
- [Preprocessing Techniques](#preprocessing-techniques)
- [Models Used](#models-used)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

To get started with the Face Scan Project, ensure you have the following prerequisites:

- Python 3.8 or higher
- Required libraries:
  ```bash
  pip install numpy opencv-python deepface retinaface tensorflow keras


## Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ankitrajsh/Face-Scan-Using-DeepFace-with-LSTM.git
   
## Prepare Your Dataset

Collect images of the person you want to analyze. Place these images in the `dataset/` directory.

## Pipeline Overview

The Face Scan project consists of the following main steps:

1. **Image Collection**: Gather multiple images of a person.
2. **Face Detection**: Use RetinaFace to detect faces in the images.
3. **Image Preprocessing**: Apply preprocessing techniques to enhance image quality.
4. **Embedding Generation**: Generate face embeddings using the DeepFace FaceNet512 model.
5. **LSTM Model Training**: Train an LSTM model to ensure consistent embeddings.
6. **Element-Wise Matching**: Ensure that all generated vectors are identical for the same individual.

## Preprocessing Techniques

Preprocessing is crucial for maintaining consistency in the generated embeddings. The following techniques are applied:

- **Brightness Normalization**: Adjusting brightness levels across images.
- **Greyscaling**: Converting images to grayscale.
- **Contrast Normalization**: Equalizing image contrast.

## Models Used

- **Face Detection**: RetinaFace
- **Embedding Generation**: DeepFace's FaceNet512
- **Refinement Model**: Long Short-Term Memory (LSTM)

## Results

The model achieves exact element-wise matching of the 128-dimensional vectors for the same individual across different images. This consistency enhances the reliability of the face recognition system.

## Contributing

Contributions are welcome! If you would like to contribute to the Face Scan project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

