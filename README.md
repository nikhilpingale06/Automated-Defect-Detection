# Automated-Defect-Detection

Report: Automated Defect Detection 

1. Introduction
In this report, we present the methodology, performance, and insights gained from 
developing a machine learning model for automated defect detection in casting 
manufacturing processes. The goal of this project was to leverage Convolutional Neural 
Networks (CNNs) to classify defective and non-defective industrial equipment based on 
images of casting products.
2. Methodology
Dataset:
The dataset consists of images of casting products, including both defective and nondefective samples.
Defective casting images contain various types of defects such as blow holes, pinholes, 
burr, shrinkage defects, etc.
Non-defective casting images represent samples without any manufacturing defects.
Model Architecture:
We used a CNN architecture for image classification:
Input Layer (120x120x3)
Conv2D Layer (16 filters, kernel size 3x3, ReLU activation)
MaxPooling2D Layer (2x2)
Conv2D Layer (32 filters, kernel size 3x3, ReLU activation)
MaxPooling2D Layer (2x2)
GlobalAveragePooling2D Layer
Dense Layer (1 unit, Sigmoid activation)
Training:
The model was trained using a training set and evaluated using a separate test set.
We utilized binary cross-entropy loss and Adam optimizer during training.
3. Model Performance
Test Accuracy: 74%
Test Loss: 0.5183
Confusion Matrix:
 Predicted
 Defective Non-Defective
Actual
Defective 165 28
Non-Defective 50 57
4. Insights and Analysis
Model Performance: The trained CNN achieved a test accuracy of 74%, indicating its 
effectiveness in distinguishing between defective and non-defective casting products.
Confusion Matrix Analysis:
True Positives (Defective correctly predicted as Defective): 165
False Negatives (Defective incorrectly predicted as Non-Defective): 28
False Positives (Non-Defective incorrectly predicted as Defective): 50
True Negatives (Non-Defective correctly predicted as Non-Defective): 57
Importance of Automation: Automating defect detection using machine learning can 
significantly reduce manual inspection time and improve accuracy compared to humanbased inspection methods.
Areas for Improvement:
Data Quality: Continuously improving the dataset quality and diversity can enhance model 
generalization.
Model Fine-Tuning: Experimenting with different CNN architectures, hyperparameters, and 
regularization techniques may further improve model performance.
Error Analysis: Investigating specific types of misclassifications (e.g., false negatives) can 
guide targeted improvements in model training and data collection.
5. Conclusion
In conclusion, the developed CNN model demonstrates promising performance for 
automated defect detection in casting manufacturing. By leveraging machine learning, we 
can enhance quality control processes, reduce production costs, and mitigate the risks 
associated with defective products. Continuous refinement and integration of such 
models into industrial workflows hold great potential for improving manufacturing 
efficiency and product quality
