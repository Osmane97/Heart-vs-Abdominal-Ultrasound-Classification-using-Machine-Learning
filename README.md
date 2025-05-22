# Heart-vs-Abdominal-Ultrasound-Classification-using-Machine-Learning
Medical ultrasound image classification using CNN and Random Forest. Includes binary classification of heart vs abdominal scans, valve state classification (open/closed), and performance improvement via data augmentation and transfer learning.

Automatically separating cardiac from non-cardiac ultrasound scans helps streamline the diagnostic process by ensuring that relevant images are correctly routed for further analysis (e.g., assessing heart valve function), while unrelated scans (like abdominal ultrasounds) are filtered out.

This classification step is particularly useful in:

Reducing human error during manual review and labeling.

Improving efficiency in large-scale imaging databases.

Serving as a pre-processing stage in AI pipelines for advanced heart condition detection.

By automating this image type recognition, clinicians can focus more on diagnosis and patient care rather than administrative sorting tasks.

This project was completed as part of a university coursework to classify ultrasound medical images using machine learning and deep learning techniques. The dataset includes both heart and abdominal ultrasound images, with labeled heart valve states (open/closed).

###  Project Overview

This notebook presents three main experiments:

1. **Heart vs Abdominal Ultrasound Classification**
   - A binary classifier distinguishes between heart and abdominal ultrasound images.
   - Two models were implemented and evaluated:
     - **Random Forest (RF)**
     - **Convolutional Neural Network (CNN)**
   - Evaluation metrics include Precision, Recall, and F1-score.
   - 5-fold cross-validation was applied for robust validation.

2. **Heart Valve State Classification (Open vs Closed)**
   - A classifier was trained only on heart images to detect whether the mitral valve is open or closed.
   - Both Random Forest and CNN were applied.
   - Evaluation includes metrics such as Confusion Matrix, Precision, Recall, F1-score, and ROC Curve.

3. **Performance Improvement**
   - Techniques such as **image augmentation** and **transfer learning** (using VGG16) were applied to improve CNN model accuracy.
   - The same test set was used throughout to ensure fair performance comparison.

###  Dataset Structure

- `heart/open`: 138 images with open mitral valves
- `heart/closed`: 80 images with closed mitral valves
- `Data_1/heart`: includes clinician-annotated segmentation masks
- `Data_1/non-heart`: 925 abdominal ultrasound images


###  Results Summary

- CNN outperformed Random Forest on heart vs abdominal classification.
- Augmented CNN and VGG16-based transfer learning improved open/closed classification results.
- Evaluation metrics showed consistent improvement across experiments.



