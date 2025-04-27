# 🦷 Oral Cancer Detection Project

## 🚀 Workflow

1. **Dataset Download and Preparation**
   - Download oral cancer dataset from Kaggle.
   - Unzip and organize images into **'cancer'** and **'non-cancer'** folders.

2. **Library Installation and Import**
   - Install essential libraries: `tensorflow`, `scikit-learn`, `matplotlib`, etc.
   - Import necessary modules for image processing, model building, and training.

3. **Data Loading and Preprocessing**
   - Load images and convert them into numpy arrays.
   - Resize all images to **260x260** pixels.
   - Label encoding:  
     - `0` → Cancer  
     - `1` → Non-cancer

4. **Train-Test Split**
   - Split dataset into training and testing sets (80% train, 20% test) using `train_test_split`.

5. **Model Building**
   - Use **EfficientNetB2** as the base model (pretrained on ImageNet).
   - Add custom dense layers on top.
   - Freeze the base model layers during initial training.

6. **Model Compilation**
   - Loss Function: `binary_crossentropy`
   - Optimizer: `Adam`
   - Metrics: `accuracy`

7. **Training**
   - Train the model with:
     - Early Stopping
     - ReduceLROnPlateau
     - Model Checkpoint (saving best model)
   - Data augmentation applied using `ImageDataGenerator`.

8. **Evaluation**
   - Evaluate the model on the test dataset.
   - Plot accuracy and loss graphs.

9. **Prediction**
   - Test the trained model on individual images.
   - Display results with prediction labels (Cancer / Non-cancer).

10. **Appendix**
    - Data Set Link : https://www.kaggle.com/datasets/zaidpy/new-oral-cancer
    - Project files link : https://drive.google.com/drive/folders/1Mwvun76Z-70Di_zieyp9hoK1tretvOiB?usp=sharing
    - Demo Video Link : https://drive.google.com/file/d/1Sx0Ki0tEs8LEP7Wb2nqb6F7BErLhBPwq/view?usp=sharing
