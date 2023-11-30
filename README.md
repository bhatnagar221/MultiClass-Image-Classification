# MultiClass-Image-Classification
The primary goal of the project is to employee transfer learning techniques, specifically utilizing the InceptionResNetV2 model, for the purpose of multi-class image classification. This project focused on the challenging task of accurately categorizing diverse dog breeds through the customization of the pre-trained model.
# Dataset Description
* The dataset used comprises of 120 breeds of dogs in total.
* Each image has a file name which is its unique id.
* Train dataset ( train.zip ): contains 10,222 images which are to be used for training our model
* Test dataset (test.zip ): contains 10,357 images which we have to classify into the respective categories or labels.
* labels.csv: contains breed names corresponding to the image id.
* sample_submission.csv: contains correct form of sample submission to be made

# Methods Employed In this Project
* Transfer Leaarning: Transfer learning is a popular deep learning method that follows the approach of using the knowledge that was learned in some task and applying it to solve the problem of the related target task. So, instead of creating a neural network from scratch we “transfer” the learned features which are basically the “weights” of the network. To implement the concept of transfer learning, we make use of “pre-trained models“.
* Pre-Trained Model: Pre-trained models are the deep learning models which are trained on very large datasets, developed, and are made available by other developers. Here we have used InceptionResNetV2 architecture, a pre-trained model known for its effectiveness in various computer vision tasks. Tailored the InceptionResNetV2 model to the specific requirements of the multi-class image classification task. Fine-tuned the pre-trained model to adapt its learned features to accurately categorize images of different dog breeds, showcasing the flexibility and adaptability of transfer learning.
* Data Preprocessing : I have used data augmentation tecnique. It’s a pre-processing technique in which we augment the existing dataset with transformed versions of the existing images. We can perform scaling, rotations, increasing brightness, and other affine transformations. This is a useful technique as it helps the model to generalize the unseen data well.
ImageDataGenerator class is used for this purpose which provides a real-time augmentation of data.a 

Description of few of its parameters that are used below:
 * rescale: rescales values by the given factor
 * horizontal flip: randomly flip inputs horizontally.
 * validation_split: this is the fraction of images reserved for validation (between 0 and 1)
