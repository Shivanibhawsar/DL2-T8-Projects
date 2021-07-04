# SIGN LANGUAGE CLASSIFICATION

In this project, I have classified the sign language symbols using the Convolutional Neural Network (CNN). After successful training of the CNN model, the corresponding alphabet of a sign language symbol will be predicted. We will evaluate the classification performance of our model using the non-normalized and normalized confusion matrices. Finally, we will obtain the classification accuracy score of the CNN model in this task.


## Dataset

In this project, I have used the American Sign Language (ASL) data set that is provided by MNIST . This dataset contains 27455 training images and 7172 test images all with a shape of 28 x 28 pixels. These images belong to the 25 classes of English alphabet starting from A to Y (No class labels for Z because of gesture motions). This dataset is in the CSV format where training data has 27455 rows and 785 columns. The first column of the dataset represents the class label of the image and the remaining 784 columns represent the 28 x 28 pixels. The same pattern is followed by the test data set.

Source for the dataset - kaggle


## Libraries Required

Some important libraries should be uploaded to read the dataset, preprocessing and visualization. These are:
- Tensorflow
- Keras
- Pandas
- Numpy
- Random
- Matplotlib
- Seaborn


## Model

- Two 2D convolution layer in sequence with input shape as (28,28,1) and relu as activation function along with dropout to avoid overfitting.
- A MaxPooling2D layer to extract most prominent features.
- Two dense layer as output layer connected sequentially with relu and softmax as its activation function respectively.


## How to run

First run 'Project final.ipynb' then run 'Random_train_images.ipynb' file.


## Result

After 30 epochs <br>
Testing  Acuuracy = 95.24%
