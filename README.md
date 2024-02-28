# Deploying-MNIST-using-PYTorch-Lightning-and-WANDB


## Overview
This project showcases the use of PyTorch Lightning to train a neural network on the MNIST dataset and leverages Weights & Biases (wandb) for experiment tracking and model management.

## Features
- Utilizes PyTorch Lightning for the modular and scalable training of deep learning models.
- Integrates wandb for real-time logging of training metrics and version control of model checkpoints.
- Implements the ONNX format for model serialization, enabling deployment across diverse platforms.

## Installation
To install the necessary dependencies for this project, run:
pip install -qqq wandb lightning torchmetrics onnx


## Structure
- `LitMLP` class: Defines the model architecture and training/validation/test steps using PyTorch Lightning's Module API.
- `MNISTDataModule` class: Handles data loading and preprocessing for the MNIST dataset.
- WandB Integration: Sets up Weights & Biases for monitoring and tracking the training process.

## Training the Model
- The `train.py` script orchestrates the training process, including model initialization, trainer configuration, and execution of the training loop.

## Model Checkpointing
- The `on_test_epoch_end` method is overridden to convert the trained model to ONNX format and log it to wandb as an artifact.


![Screenshot 2024-02-28 150816](https://github.com/saahil1801/Deploying-MNIST-using-PYTorch-Lightning-and-WANDB/assets/84408557/c03df0ce-d8ff-4fc9-b0da-f168d429ba0b)
![Screenshot 2024-02-28 150708](https://github.com/saahil1801/Deploying-MNIST-using-PYTorch-Lightning-and-WANDB/assets/84408557/730f38da-4233-4363-be66-1d95784971a0)
![Screenshot 2024-02-28 150735](https://github.com/saahil1801/Deploying-MNIST-using-PYTorch-Lightning-and-WANDB/assets/84408557/85fbf056-40fa-4bc1-a10e-0e1df908d303)


## Experiment Tracking
WandB dashboards provide insights into the training process, with metrics such as accuracy and loss visualized in real-time.

## Contributing
Contributions are welcome. Please submit an issue or pull request with your proposed changes or enhancements.

## License
This project is licensed under the terms of the MIT license.

## Acknowledgments
- Thanks to the creators of the PyTorch Lightning framework and Weights & Biases platform for their fantastic tools.
- MNIST dataset creators for providing a benchmark dataset for the machine learning community.



For any questions or support, please open an issue on this repository.


```

Ensure that you include all relevant scripts and files in the repository and provide a detailed guide on how to replicate the model's training and deployment. If there are any specific requirements or steps needed to run the code, these should be included in the README as well.
