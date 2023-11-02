# Face Recognition System

## Overview

This face recognition system is designed for low-powered CPUs like Raspberry Pi and NVIDIA Jetson Nano. It boasts fast training times and the ability to recognize faces efficiently. Below are the instructions to set up and use the system.

## Installation

1. Clone or download this repository to your low-powered CPU device.
2. Navigate to the project directory.
3. Install the required Python packages using `requirements.txt`. Run the following command:

```
pip install -r requirements.txt
```


## Usage

### 1. Training the Model

- Execute `train.py` by running

```
python train.py
```

- In the GUI that appears, input an ID and a name for the person you want to add to the system.
- Click the "Take Picture" button to capture an image of the person's face.
- Repeat the above steps for each individual you want to train the model with.
- After capturing images for all individuals, run the "Train Model" command to train the facial recognition model.

### 2. Recognizing Faces

- Before running `recognize.py`, ensure you update the label names in the code to match the individuals trained in the previous step.
- Run `recognize.py` using the following command:

```
python recognize.py
```

- The system will utilize the trained model to recognize faces and display the results.


## Note

- Make sure your CPU-based device is properly configured to access a camera for image capture.
- If you are using a Raspberry Pi, it's recommended to use a dedicated camera module for better results.
- This system is primarily for educational and experimental purposes. It may not meet the performance standards of high-end facial recognition systems used in security applications.

## License

This project is licensed under the MIT License. Refer to the [LICENSE](https://rem.mit-license.org/) file for more details.



Feel free to modify and enhance this system to meet your specific needs. If you have any questions or require assistance, please don't hesitate to reach out.