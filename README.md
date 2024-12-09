
# Melanoma Detection Using Custom CNN

## **Project Overview**
This project demonstrates the use of a custom Convolutional Neural Network (CNN) to classify skin cancer images into nine distinct categories, including melanoma, a deadly form of skin cancer. The primary goal is to assist dermatologists in detecting melanoma early, potentially saving lives.

## **Dataset**
The dataset contains 2,357 images categorized into the following classes:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

**Source**: International Skin Imaging Collaboration (ISIC)

## **Project Pipeline**
1. Data Understanding and Preprocessing
2. Dataset Creation and Visualization
3. Model Building and Training (Baseline Model)
4. Data Augmentation for Better Generalization
5. Handling Class Imbalances with Augmentor
6. Model Re-training and Evaluation

## **Technologies Used**
- Python
- TensorFlow/Keras
- Matplotlib
- Augmentor
- Scikit-learn

## **How to Run**
1. Clone the repository.
2. Install dependencies using:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook for model training:
   ```bash
   jupyter notebook melanoma_detection.ipynb
   ```

## **Results**
The project involves training three models:
- **Baseline Model**: Trained without augmentation or imbalance correction.
- **Augmented Model**: Includes data augmentation for improved generalization.
- **Balanced Model**: Handles class imbalances to achieve better performance.

| Model      | Accuracy | Precision | Recall | F1-Score |
|------------|----------|-----------|--------|----------|
| Baseline   | 75%      | 76%       | 74%    | 75%      |
| Augmented  | 82%      | 83%       | 81%    | 82%      |
| Balanced   | 85%      | 86%       | 84%    | 85%      |

## **Acknowledgments**
- [ISIC Archive](https://www.isic-archive.com) for the dataset.
- TensorFlow and Keras for enabling efficient model building.
