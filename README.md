# [**Cats vs Dogs Classification:CNN**](https://www.kaggle.com/c/dogs-vs-cats)

#### **Notebooks:**

- [**Cats vs Dogs Classification**](https://github.com/ThinamXx/Cats.vs.Dogs_Classification/blob/master/Cat%20vs%20Dog%20Classification.ipynb)
  - In this Notebook, I have used Convolutional Neural Network to prepare the Model. The accuracy of the Model is in range of 80% on Training data and Validation data.
  
- [**Cats vs Dogs Classification with Imagenet and InceptionV3**](https://github.com/ThinamXx/Cats.vs.Dogs_Classification/blob/master/CatvsDog%20Classification%20with%20Imagenet.ipynb)
  - In this Notebook, I have used Convolutional Neural Network to prepare the Model. The accuracy of the Model is above 95% on Training data as well as Validation data.

**Convolutional Neural Network**
- In deep learning, a convolutional neural network is a class of deep neural networks, most commonly applied to analyzing visual imagery. They are also known as shift invariant or space invariant artificial neural networks, based on their shared-weights architecture and translation invariance characteristics.

**Imagenet**
- The ImageNet project is a large visual database designed for use in visual object recognition software research. More than 14 million images have been hand-annotated by the project to indicate what objects are pictured and in at least one million of the images, bounding boxes are also provided.

**InceptionV3**
- InceptionV3 is a convolutional neural network that is 48 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. You can use classify to classify new images using the Inception-v3 model.

#### **Getting the Data**
- In this Project, I have downloaded the data using the link mentioned below. You can manually download the data from [Kaggle](https://www.kaggle.com/c/dogs-vs-cats/data). I am using Google Colab for this Project, so the act of reading the data might be different in different platforms.

```javascript
!wget --no-check-certificate \
    "https://download.microsoft.com/download/3/E/1/3E1C3F21-ECDB-4869-8368-6DEBA77B919F/kagglecatsanddogs_3367a.zip" \
    -O "/tmp/cats-and-dogs.zip"
```

#### **Snapshot of the Data**
- I have presented the 8 pictures of Dogs and 8 pictures of Cats which is presented below:

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1597395757/Cats_g3xbvy.png)

**Data Augmentation**
- Data augmentation is a strategy that enables practitioners to significantly increase the diversity of data available for training models, without actually collecting new data. Data augmentation techniques such as cropping, padding, and horizontal flipping are commonly used to train large neural networks.

```javascript
ImageDataGenerator(rescale=1./255,
                                   rotation_range=40,
                                   width_shift_range=0.2,
                                   height_shift_range=0.2,
                                   shear_range=0.2,
                                   zoom_range=0.2,
                                   horizontal_flip=True,
                                   fill_mode="nearest")
```

**Snapshot of the Loss and Accuracy score with Transfer Learning**

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1597396086/Vali_y547gk.png)

**Snapshot of the Output of Model**

![Image](https://res.cloudinary.com/dge89aqpc/image/upload/v1597396296/AAAA_unl2fs.png)
