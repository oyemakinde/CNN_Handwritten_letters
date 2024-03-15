# CNN_Handwritten_letters
The purpose of this project was to train a Convolutional Neural Network (CNN) using TensorFlow with Keras to recognize handwritten English letters. The dataset consisted of both training and test images, along with their corresponding labels.

Each image in the dataset was sized 28x28 pixels, with the pixel values representing the grayscale level. A pixel value of 0 indicated black, while a value of 255 represented white. The dataset encompassed a total of 297,960 images for training and 74,490 images for testing. Each image had a label associated with it, indicating the specific letter of the alphabet it represented.

The labels were represented as arrays of 26 integer values, with all values set to zero except for the position corresponding to the letter in the image. For instance, the label for the letter "B" (which is the second letter in the alphabet) would have zeros in all positions except the second position, where it would be set to 1. Similarly, the label for the letter "S" (the nineteenth letter) would have zeros in all positions except the nineteenth position.

To begin the project, the provided zip file needed to be uncompressed, revealing the following files:

train_images.npy
train_labels.npy
test_images.npy
test_labels.npy
These files contained the necessary data for training and testing the CNN. After uploading the files to Google Drive and mounting it in the Colab file system, the data could be loaded into NumPy tensors using the following commands:

train_images = np.load(......insert train images file name and path here .........)
train_labels = np.load(......insert train labels file name and path here .........))
test_images = np.load(......insert test images file name and path here .........))
test_labels = np.load(......insert test labels file name and path here .........))

By leveraging these data files and employing the appropriate TensorFlow and Keras functions, the CNN model could be trained to accurately recognize handwritten English letters.
