# Color-Invariant-Saree-Recognition
Color-invariant saree design recognition using ResNet18 and contrastive learning
# DeepLure – Color-Invariant Saree Design Recognition

## Project Overview

This project focuses on identifying saree designs regardless of their color variations.

The objective is to build an image recognition system that compares saree patterns and identifies visually similar designs even when their colors are different.

## Technologies Used

- Python
- PyTorch
- Torchvision
- ResNet18 (pretrained model)
- Kaggle Notebook
- Matplotlib

## Methodology

1. Collected and prepared saree images.
2. Applied image preprocessing and augmentation.
3. Used a pretrained ResNet18 model for feature extraction.
4. Created 128-dimensional image embeddings.
5. Applied contrastive learning using NT-Xent loss.
6. Used cosine similarity for image comparison.
7. Implemented image identification and verification.

## Model Details

- Backbone: ResNet18
- Embedding Dimension: 128
- Loss Function: NT-Xent (Contrastive Loss)
- Optimizer: AdamW
- Training Epochs: 15
- Batch Size: 16

## Evaluation Results

| Metric | Result |
|---|---:|
| Recall@1 | 80% |
| Recall@5 | 100% |
| Verification Accuracy | 98% |
| Verification Precision | 96.15% |
| Verification Recall | 100% |
| Verification F1 Score | 98.04% |

## Limitations

- The dataset contained only 165 images.
- Reliable real-world saree design labels were not available.
- Color variations were generated using image augmentation.
- Evaluation was performed using controlled image transformations.
- Results do not establish real-world recognition accuracy across independently photographed sarees.

## Future Improvements

- Use a larger dataset with verified design labels.
- Test with real saree images captured under different lighting and angles.
- Improve the model using more challenging training examples.
- Evaluate performance using independent real-world test images.

## Note

This project was developed as part of an AI Engineer assessment. The evaluation results represent the controlled experimental setup described in the notebook.
