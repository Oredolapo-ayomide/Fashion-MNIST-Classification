# Fashion MNIST CNN — Python & R Implementation

## Overview
This project implements a **Convolutional Neural Network (CNN)** to classify images from the **Fashion MNIST dataset**.  
It is implemented in **both Python** and **R (with Keras & TensorFlow backend)** to demonstrate cross-language deep learning workflows.  

The dataset contains **70,000 grayscale images** in 10 fashion categories (e.g., shirts, shoes, bags). Each image is **28x28 pixels**.

---

## Repository Structure
```
.
├── train_predict_fashion_mnist.py     # Python implementation
├── Fashion_MNIST.R                    # R implementation

```

---

### Python Requirements
- **Python** 3.8 or later  
- Packages:
  - `tensorflow`
  - `keras`
  - `numpy`
  - `matplotlib`
  - `scikit-learn` (optional for metrics)

Install dependencies:
```bash
pip install -r requirements.txt
```
Or manually:
```bash
pip install tensorflow keras numpy matplotlib scikit-learn
```

---

### R Requirements
- **R** version 4.0 or later  
- **RStudio** (recommended)  
- Packages:
  - `keras`
  - `tensorflow`

Install packages in R:
```r
install.packages("keras")
install.packages("tensorflow")
library(keras)
library(tensorflow)
install_keras() # Sets up TensorFlow backend
```
**Note:** `install_keras()` will also install Python and TensorFlow. 

---

## Running the Code

### Python
1. Open a terminal or command prompt  
2. Navigate to the project directory:
   ```bash
   cd path/to/project
   ```
3. Run:
   ```bash
   python train_predict_fashion_mnist.py
   ```
4. The script will:
   - Load the dataset
   - Preprocess images
   - Build & train the CNN model
   - Display training accuracy and loss
   - Evaluate on test data

---

### R
1. Open **RStudio**  
2. Open `Fashion_MNIST.R`  
3. Ensure the `keras` and `tensorflow` packages are installed (see above)  
4. Click **Run** or use:
   ```r
   source("Fashion_MNIST.R")
   ```
5. The script will:
   - Load the dataset using `dataset_fashion_mnist()`
   - Preprocess images and labels
   - Build & train the CNN model
   - Output training progress and test accuracy

---

## Troubleshooting

### Python Issues
- **`ModuleNotFoundError`** → Run `pip install <package>` to install the missing package.  
- **TensorFlow not using GPU** → Ensure you have installed the GPU version of TensorFlow and proper CUDA drivers.  

### R Issues
- **Error: no function 'to_categorical'** → Make sure `library(keras)` is loaded and your `keras` package is updated:
  ```r
  install.packages("keras")
  library(keras)
  ```
- **TensorFlow not found** → Run `install_keras()` again.

---

## Output
The scripts will output:
- Training and validation accuracy/loss per epoch  
- Final test accuracy and loss   
---
