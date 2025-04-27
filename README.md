# Blood_group_detection_ML_proj
Blood Group Detection from Images 🩸🔍
Aim
To create an automated deep learning model that can detect a person’s blood group from image data, making blood group verification non-invasive, fast, and reliable.

Introduction
Blood group identification is a critical step in medical procedures. Traditional methods involve blood sampling, which can be invasive and uncomfortable, especially for hemophobes (people afraid of blood).
This project offers a solution using deep learning: predicting blood groups from images of blood group labels/tags.
It is particularly helpful for cross-verifying negative blood groups, where accuracy is vital.

Methodology (Step-by-Step)
1. Dataset Preparation
Unzipped the archive containing blood group images.

Organized original dataset into proper folders by blood group class.

2. Data Preprocessing
Plotted class distribution to check for imbalance among different blood groups.

Balanced the dataset by undersampling the classes to have an equal number of images per blood group.

3. Data Splitting
Split the dataset into training (80%) and testing (20%) sets.

Used ImageDataGenerator for real-time data augmentation (rotation, shift, zoom).

4. Model Building
Built a Convolutional Neural Network (CNN) using TensorFlow/Keras.

Included layers like Conv2D, MaxPooling2D, Dropout, and Dense.

Compiled the model with categorical_crossentropy loss and Adam optimizer.

5. Model Training
Trained the CNN model on the prepared dataset over multiple epochs.

Monitored accuracy and loss during training to avoid overfitting.

6. Evaluation
Evaluated the model using:

Confusion matrix

Classification report (precision, recall, F1-score)

Visualized performance with accuracy and loss plots.

Conclusion
This project successfully demonstrates that blood group prediction from images is achievable with high accuracy using deep learning techniques.
It reduces dependency on invasive blood sampling and provides a safe, quick, and user-friendly method for identifying blood groups.

Use Cases
✅ For Hemophobes: No need for blood draws—simple image recognition.

✅ For Hospitals and Blood Banks: Fast verification of blood groups, especially critical for rare and negative blood groups.

✅ In Emergencies: Quick identification without traditional lab tests.
