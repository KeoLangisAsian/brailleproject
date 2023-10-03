# Braille Project

 This project was designed to help people read braille using machine learning and AI

![In this repository, images that were run through the model were added](direct image link here)

## The Algorithm

This project uses a retrained resnet-18 model which has been trained by the dataset provided in the repository. The PyTorch model has been converted to ONNX format for use on the Jetson nano.

## Running this project

1.	Set up the jetson-inference project linked [here](https://github.com/dusty-nv/jetson-inference)
2.	change directories into this repository
3.     run the following command:
imagenet.py --model=models/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=braille_dataset/labels.txt input_file_name output_file_name
