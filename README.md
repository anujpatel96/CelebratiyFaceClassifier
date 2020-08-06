# CelebratiyFaceClassifier
This project aims to predict the name of the celebrity by the image. It is a classic classification project which has five different class to predict. Nowadays “Neural Networks” are dominant in the Image processing domain but the main idea behind this project is to show that with the help of simple classification model such as SVM and Logistic Regression, we can get good accuracy for the Image classification problems. First, I divided the project into three parts.
1> Data Collection
2> Data Cleaning and Model Building
3> Model Deployment

For the first part I had to collect the images of different celebrities. I picked my favourite sport persons from different sports and search their images on Google. Then I used “Image Downloader” extension to download all images with single click. After getting all the images I made five classes of the data. 
For the data cleaning in the second part I manually deleted some of the images in which the face was not clear or obstructed. Then with the help of “openCV” library I defined two functions, first to crop the face out of the image and second to detect eyes and mouth on the cropped image. Then I tried different classification model such as SVM, Random Forest and Logistic Regression to check which works best for my project. I also used GridSeachCV and KFold to choose the best model and best parameters for the model. I achieved result shown as below.
| Model  | Best_score |
| ------------- | ------------- |
| SVM | 0.80 |
| Random Forest | 0.63 |
| Logistic Regression | 0.81 |

For the third part, I created a pickle file and with the help of python Flask I build my local server to run my local website and deployed the model on the website to predict the class of new images. The UI of the model running on a local website is shown as below. 
