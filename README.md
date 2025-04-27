📜 License and Copyright

© 2025 Rajeshwari Tukaram Golande. All rights reserved.

This project is for educational and personal use only. Commercial use is prohibited without permission.


Blood Group Detection from Fingerprint Images 🩸🔍

Aim
To create an automated deep learning model that can detect a person’s blood group from fingerprint images, making blood group verification non-invasive, fast, and reliable.

Introduction
Blood group identification is a critical step in medical and emergency services. Traditional methods involve blood sampling, which can be invasive and uncomfortable, especially for hemophobes (people afraid of blood).
This project provides an image-based solution using deep learning: predicting blood groups from fingerprint images.
It is particularly useful for cross-verifying rare negative blood groups, where 100% accuracy is essential.

Dataset
Source: Kaggle - Fingerprint Based Blood Group Dataset

Description:
The dataset contains fingerprint images labeled with corresponding blood groups (A+, A-, B+, B-, AB+, AB-, O+, O-).
Each class folder contains multiple fingerprint images collected for that blood group.

Methodology (Step-by-Step)
1. Dataset Preparation
Downloaded and extracted the fingerprint dataset from Kaggle.

Organized images into folders by blood group labels.

2. Data Preprocessing
Visualized class distribution: Initially, some blood groups had more images than others.

Balanced the dataset by:

Undersampling all classes to match the class with the fewest images.

Using the same number of images for each blood group to avoid bias during training.

Plotted the balanced class distribution to confirm uniformity.

3. Data Splitting
Split the dataset into:

80% Training set

20% Testing set

Applied real-time data augmentation (rotation, zoom, shift) using TensorFlow’s ImageDataGenerator to artificially expand the training set.

4. Model Building
Built a Convolutional Neural Network (CNN) with:

Multiple Conv2D layers + MaxPooling layers

Dropout layers to reduce overfitting

Fully connected Dense layers for classification

Compiled the model using Adam optimizer and categorical_crossentropy loss.

5. Model Training
Trained the model for several epochs on the balanced dataset.

Monitored training and validation accuracy to ensure the model was learning appropriately.

6. Evaluation
Evaluated model performance using:

Confusion Matrix

Classification Report (Precision, Recall, F1-Score)

Achieved an accuracy of approximately XX% (replace XX with your actual model accuracy).

Visualized training/validation accuracy and loss trends.

Conclusion
This project demonstrates that blood group prediction from fingerprint images can be achieved with deep learning techniques, offering a non-invasive, fast, and reliable alternative to traditional blood sampling.
Balancing the dataset helped the model learn fairly across all blood groups, without favoring the majority classes.

Use Cases
✅ For Hemophobes: No needles, no blood draws—only fingerprint images needed.

✅ For Hospitals and Blood Banks: Rapid and non-invasive blood group verification.

✅ Emergency Situations: Immediate identification without waiting for lab results.

✅ Cross-verification of Negative Blood Groups: Avoids errors where negative groups are critical.

🚀 Tech Stack
Python 🐍

TensorFlow/Keras 🤖

NumPy, Matplotlib, Seaborn 📊

Scikit-learn 🛠️

