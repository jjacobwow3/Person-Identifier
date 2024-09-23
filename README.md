Cleans images in a way that is suitable for our classifier
Identifies a photo with a face.
Face is defined by haar cascades to detect if a face and 2 eyes are visible or not
if they are then image is kept, discarded otherwise.
Majority of cleaning is done using Python but some manual work may be required.
Generates cropped images of faces

use cropped images and wavelt transform to help with image identification
using wavelet transform and a raw pixel image to create X and use class labels as y for model training

simple SVM model is used to perform image classification
GridSearchCV is used to try diferent models with different params to com eup with the most accurate model.
sklearn classification_report is used to check the performance.
Once the best model is selected it is evaluated on X_test and y_test.
Confusion matrix is used with seaborn visualization to understand the errors of each class.

In the end pkl model is produced.

HOW TO USE
Run server.py in the server folder, Then run app.html in the UI folder.
