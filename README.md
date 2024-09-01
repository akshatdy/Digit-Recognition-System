# Digit Recognition System

## Project Overview

This project involves the development of a speech-based digit recognition system using Hidden Markov Models (HMM). The system is designed to recognize spoken digits (0-9) and supports both pre-recorded audio files and live speech input for testing. The system has been trained using 20 utterances per digit and is tested with 10 utterances per digit.

## Features

- **Data Preprocessing**: Functions like `normalize_data()`, `calculate_energy_of_frame()`, and `mark_checkpoints()` prepare the audio data for analysis.
- **Model Training**: Utilizes Hidden Markov Models (HMM) with functions such as `train_model()`, `re_estimation()`, and `viterbi_algo()` to build accurate models for each digit.
- **Testing and Recognition**: Functions `recognize_digit()`, `testing()`, and `live_test_HMM()` handle the recognition of digits using pre-recorded files or live input.
- **Distance Calculation**: Includes `minTokhuraDistance()` to measure the similarity between test inputs and trained models.
- **Clustering**: Functions like `KMeans()` and `LBG()` are used for vector quantization during the model training process.
- **Flexible Testing**: The system allows testing with both pre-recorded files and live recordings, making it adaptable to different scenarios.

## Prerequisites

- **Visual Studio 2010**: The project is developed in C++ and requires Visual Studio 2010 for compilation and execution.

  Ensure Visual Studio 2010 is installed on your system before running the project.


## Installation
- Ensure Visual Studio 2010 is installed on your system.
- Download and extract the project files from the repository.

## How to Run
1. **Open the Project**:
   - Navigate to the extracted folder.
   - Double-click on the `234101059_digitrecognition.sln` file to open the project in Visual Studio 2010.

2. **Build the Project**:
   - In Visual Studio, go to `Build > Build Solution` to compile the project.

3. **Run the Project**:
   - Press `F5` to start the project. After training, you’ll be prompted to choose between testing with pre-recorded files or live testing.
   - The system will display predictions for each test case based on your selection.