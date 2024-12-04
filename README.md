# Automated-Plant-Seedling-Classifier

## Introduction
The goal of this project is to build a deep learning model capable of classifying 12 different plant species. Early identification of plant seedlings can help in:
- Disease control
- Resource optimization
- Better decision-making for farmers and researchers
---

## Dataset
- **Source**: [V2 Plant Seedlings Dataset (Kaggle)](https://www.kaggle.com/datasets/vbookshelf/v2-plant-seedlings-dataset)
- **Classes**: 12 plant species (e.g., Black-grass, Charlock, Cleavers, etc.)
- **Total Images**: 5,533 (cleaned and augmented)
---

## Model
This project leverages transfer learning with the **ResNet18** architecture:
- Pre-trained on ImageNet
- Modified final layer to output predictions for 12 classe

### Data Preprocessing
- Resize images to 224x224 pixels
- Normalize pixel values
- Apply data augmentation
---

## Results
- **Accuracy on Test Set**: 92%
- **Evaluation Metrics**:
  - Precision
  - Recall
  - F1-score
---

## Challenges
1. **Class Imbalance**: 
   - Certain classes had significantly fewer samples.
2. **Visual Similarity**: 
   - Some plant species were visually difficult to distinguish.
3. **Limited Data**: 
   - Data augmentation was crucial to improve model robustness.
