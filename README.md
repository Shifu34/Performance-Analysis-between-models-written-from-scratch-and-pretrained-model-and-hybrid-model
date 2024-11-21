
# Performance Analysis: Custom, Pretrained, and Hybrid Models

This Jupyter Notebook provides a comprehensive performance analysis of three types of machine learning models:
1. Models written from scratch.
2. Pretrained models.
3. Hybrid models (a combination of scratch-built and pretrained components).

## Key Components
### 1. Data Preparation
The notebook explains the preprocessing techniques applied to the dataset, including normalization, data augmentation, and splitting into training and testing sets.

### 2. Model Design and Types
- **VGG-like Model (Scratch)**: A custom implementation inspired by the VGG architecture, designed and trained from scratch.
- **ResNet-like Model (Scratch)**: A custom implementation inspired by ResNet, including skip connections, trained from scratch.
- **Hybrid Model**: A combination of custom architecture and pretrained layers for feature extraction, blending scratch-built and pretrained techniques.
- **PyTorch Built-in VGG Model**: A pretrained VGG model from PyTorch’s library, fine-tuned for the given dataset.
- **PyTorch Built-in ResNet Model**: A pretrained ResNet model from PyTorch’s library, fine-tuned for the dataset.

### 3. Training and Evaluation
Each model was trained with identical datasets and similar hyperparameter settings (e.g., learning rate, batch size) for a fair comparison. The evaluation used metrics such as accuracy, precision, recall, and F1-score.

### 4. Results and Comparison
#### Accuracies Achieved:
- **VGG-like Model (Scratch)**: 74.27%
- **ResNet-like Model (Scratch)**: 83.49%
- **Hybrid Model**: 78.44%
- **PyTorch Built-in VGG Model**: 72.01%
- **PyTorch Built-in ResNet Model**: 76.92%

### Observations
- The **ResNet-like Model (Scratch)** achieved the highest accuracy, demonstrating the strength of skip connections and residual learning.
- The **Hybrid Model** balanced performance, combining the flexibility of custom models with the robustness of pretrained components.
- Pretrained models (e.g., PyTorch Built-in VGG and ResNet) showed slightly lower performance, potentially due to suboptimal fine-tuning or dataset mismatch.


## Prerequisites
- Python 3.x
- Required libraries:
  - PyTorch (depending on model implementation)
  - NumPy
  - Matplotlib
  - pandas
  - scikit-learn
- Dataset CIFAR-10

## How to Use
1. Clone this repository or download the notebook.
2. Install the required dependencies using `pip install -r requirements.txt` (if provided).
3. Open the notebook in a Jupyter environment.
4. Follow the instructions to run each cell and understand the analysis.

## Author
- Name: Shafqat Mehmood
- Contact: shafqat129.mehmood@gmail.com

## License
This project is licensed under the MIT License - see the LICENSE file for details.

