# Transformer Architecture for Handwritten Text Recognition 

## Overview

This project introduces a Handwritten Text Recognition (HTR) system implemented using PyTorch and trained on various offline HTR datasets including Bentham, IAM, Rimes, Saint Gall, and Washington. The system is designed to recognize the text contained within images of segmented text lines. The heart of this project relies on the transformer architecture, a powerful neural network architecture known for its effectiveness in sequence-to-sequence tasks. By leveraging transformer architecture, the model achieves improved performance in handwritten text recognition.

## Supported Datasets

- Bentham
- IAM
- Rimes
- Saint Gall
- Washington

## Requirements 

Ensure you have the following requirements installed:

```bash
pip install opencv-python editdistance torch==1.5.0

```

## Command Line Arguments

- `--source`: dataset/model name (bentham, iam, rimes, saintgall, washington)
- `--transform`: transform dataset to the HDF5 file
- `--image`: prediction on a single image with the source parameter
- `--train`: train model using the source argument
- `--test`: evaluate and predict model using the source argument
- `--norm_accentuation`: discard accentuation marks in the evaluation
- `--norm_punctuation`: discard punctuation marks in the evaluation
- `--epochs`: number of epochs
- `--batch_size`: number of the size of each batch
- `--lr`: Learning rate

## Evaluation Results
- **Character Error Rate:** 0.101 (on average, it makes one mistake in every 10 characters)
- **Word Error Rate:** 0.238 (on average, it makes one mistake in every 4 words)
- **Sequence Error Rate:** 0.758 (on average, it gets about 3 out of 4 lines of text correct)

## Result Interpretation

The evaluation results showcase the performance of the HTR system:

![Output avi gif](https://github.com/pthengane/Handwritten-Text-Transformer/blob/master/Results/HTR_Results.gif)

## Acknowledgement
This project builds upon existing research in the field of handwritten text recognition. We would like to express our appreciation to the developers of the datasets used in this project. Their contributions have been invaluable in the development of this system.

Feel free to explore, contribute, and adapt the project for specific use cases.


