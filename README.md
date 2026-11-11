# Music-Mood-Classification-Using-Deep-Learning

## Overview

This project explores the use of deep learning to classify music based on mood. It uses audio processing techniques to convert music files into Mel spectrograms, which are then used as input to a pretrained ResNet50 model.

The aim was to experiment with different audio-processing techniques, dataset preparation methods and model-training approaches to explore how effectively music could be classified into four mood categories.

This was an experimental university project. The model did not achieve the accuracy I was aiming for, but the project provided practical experience with audio processing, transfer learning and model evaluation.

## Project Workflow

The notebook covers the following stages:

1. **Audio processing:** Loading audio files, resampling, converting to mono, and splitting audio into smaller chunks.
2. **Feature extraction:** Generating Mel spectrograms from the audio chunks.
3. **Dataset preparation:** Organising the spectrograms into four classification categories and preparing training and validation datasets.
4. **Data augmentation:** Experimenting with techniques such as frequency masking, time masking, waveform shifting and noise addition.
5. **Model training:** Using a pretrained ResNet50 architecture with a modified classification layer to predict one of four classes.
6. **Evaluation:** Examining model performance using accuracy, confusion matrices and precision-recall curves.

## Technologies and Libraries

- Python
- Google Colab
- PyTorch
- Torchvision
- Torchaudio
- NumPy and Pandas
- Matplotlib and Seaborn
- Scikit-learn

## Dataset

This project uses the 4Q Audio Emotion Dataset, developed by the Music Information Retrieval research group at the University of Coimbra.

The dataset contains audio clips annotated into four emotional quadrants based on Russell's Circumplex Model of Affect.

Source: Music Information Retrieval – Datasets

Dataset: 4Q Audio Emotion Dataset (2018)

### Dataset Reference

Panda R., Malheiro R. & Paiva R. P. (2018). “Novel audio features for music emotion recognition”. IEEE Transactions on Affective Computing (IEEE early access). DOI: 10.1109/TAFFC.2018.2820691.

Panda R., Malheiro R., Paiva R. P. (2018). “Musical Texture and Expressivity Features for Music Emotion Recognition”. 19th International Society for Music Information Retrieval Conference – ISMIR 2018, Paris, France.

The dataset is not included in this repository. Users must obtain it separately and configure the relevant file paths in the notebook.
Following is the link to the dataset: https://mir.dei.uc.pt/downloads.html

## Running the Notebook

The notebook was developed using Google Colab.

1. Open the `.ipynb` file in Google Colab.
2. Obtain the required dataset and upload or place it in your Google Drive.
3. Update the dataset and Google Drive paths to match your own folder structure.
4. Run the notebook cells in order.

The notebook includes the audio-processing, dataset preparation, training and evaluation stages. Training time will depend on the available hardware and dataset size.

## Credits and Acknowledgements

This project was developed as part of university coursework.

- **University starter material:** Parts of the implementation were based on starter code and material provided during coursework, which were subsequently modified and extended.
- **External resources:** Some audio-processing and model-training code was adapted from online examples and tutorials. The original source details for every adapted snippet were not retained.
- **AI assistance:** Google Gemini was used through Google Colab to assist with parts of the implementation, code modifications, debugging and experimentation.

The notebook represents an experimental implementation incorporating my own work, coursework material, adapted examples and AI-assisted development.

## Limitations

The model did not achieve the desired classification accuracy. The results should therefore be treated as experimental rather than as a reliable music mood prediction system.

The project is intended for educational and portfolio purposes, not as a finished or production-ready application.
