# Traffic Signs Detection and Classification

This is a Python program that uses various computer vision techniques to detect and classify traffic signs. The program uses the OpenCV library to process and manipulate images, the Numpy library to perform mathematical operations, the Matplotlib library to visualize data, and the Pandas library to manage datasets. The Tqdm library is used to display progress bars, and the Scikit-learn library is used for machine learning tasks such as PCA and SVM.

The program reads the training and test datasets from the "gtsrb-german-traffic-sign" directory, which is stored in the "MyDrive/Colab Notebooks/Traffic Signs Detection and Classification" directory of Google Drive. The program uses the information in the Train.csv and Test.csv files to prepare the data for processing.

The program includes the implementation of color mapping techniques, such as hue and saturation lookup tables, to extract color information from the images. The images are first converted to the HLS color space and then resized to 200x200. The hue and saturation channels are then scaled and passed through lookup tables to extract red, blue, and yellow regions from the images. The resulting binary images are then used to calculate the HOG (Histogram of Oriented Gradients) features.

The HOG features are then processed using PCA (Principal Component Analysis) to reduce the dimensionality of the data. The processed features are then passed to an SVM (Support Vector Machine) for classification.

The Main function is the entry point of the program, which takes a metadata file as an argument and returns the list of features and labels. The function loops through all the images in the metadata file, extracts the color information and HOG features, processes the data, and trains the SVM model.

# Usage

To run the program, simply call the Main function with the metadata file as an argument, e.g. Main(train_meta). The function returns the list of features and labels, which can be used for further analysis and visualization.
