colab:- https://colab.research.google.com/drive/15L3MEyXZSHoPsaRd20WDPWHphBg7p6FW?usp=sharing

This project aims to classify brain tumor images using deep learning techniques. The project is designed to be beginner-friendly and easy to understand. Here is an explanation of the project in beginner-friendly language:

Data Preprocessing: The project starts by preparing the dataset for training. The brain tumor dataset is provided in a zip file, which is extracted and organized into a main directory. The number of classes and their names are checked, and the distribution of images among different classes is visualized using a pie chart.

Image Preprocessing: The images are preprocessed to improve the quality and focus on the brain region. Each image is cropped to include only the brain contour using image processing techniques. The cropped images are then resized to a consistent size.

Data Loading and Augmentation: The preprocessed images are loaded into the project using an ImageDataGenerator, which performs data augmentation techniques such as rotation, shifting, scaling, and flipping. This helps to increase the diversity and variability of the training data.

Model Building: The deep learning model used in this project is based on the ResNet50V2 architecture, which is a pre-trained model known for its effectiveness in image classification tasks. The base model is loaded and frozen, meaning its weights are not updated during training. A new model is created by adding a Global Average Pooling layer, followed by a dense layer with ReLU activation, and a final dense layer with softmax activation for classification.

Model Training: The model is compiled with appropriate loss and optimizer functions. It is then trained on the augmented training data and validated on the validation data. The training process involves iterating over the data for a fixed number of epochs, adjusting the model's weights to minimize the loss and improve accuracy.

Training History: The training history, including loss and accuracy metrics for both training and validation sets, is recorded and stored in a pandas DataFrame. This history can be used to analyze the model's performance over epochs.

Visualization: The training and validation loss and accuracy are plotted using matplotlib to provide a visual representation of the model's learning progress. This helps in understanding how well the model is training and if there is any overfitting or underfitting.

Prediction Visualization: Lastly, a random sample of images from the validation set is chosen and their predictions are displayed along with the original class labels. This allows you to see how well the model is performing on unseen data.
