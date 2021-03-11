# Binary Classification model (for cat / not cat images recognition). 
# 4-Layers Neural Network.


**Input:** dataset of images, labeled as 1/0 (cat / not cat). 209 training and 50 test images.

**Data preprocessing:**
- **Flatten**: Every image has size of 64px * 64px * 3 layers (RGB). It is 4096 px with 3 features for each. That is 12 288 features in total for each image.
- **Standardize**: as every feature has value of [0, 255] (the intensity of red, green or blue color), we standardize it by dividing every element on 255.

**Model:**
Neural Network (4 layers):
- Optimization algorithm: Batch Gradient Descent
- Activation functions: layer 1, 2, 3 – ReLU, and layer 4 – sigmoid (as it is binary classification problem)

Hyperparameters of the Neural Network:
-	Depth: 3 hidden layers
-	Width: layer1 = 20, layer2 = 7, layer3 = 5, output (y) layer: layer4 = 1
-	Number of iterations: 3000
-	Learning rate: 0.0075

**Result:** prediction accuracy – 78% on the test dataset.

**Python packages used for creating the model:** numpy
