# Brain-Tumor-Detection-with-CNN

##  Objective

We work with a dataset containing MRI scans divided into four classes, three tumor classes (Pituitary, Glioma, and Meningiome) and one class representing normal brain scans. The aim of this notebook is to use Convolutional Neural Networks (CNN) to distinguish between normal brain scans and those containing any of the tumor classes. To achieve this goal we build, and tune, a deep CNN and we also use a pretrained convolutional network (Mobilnet).

##  About the dataset

What is a brain tumor?

A brain tumor is a collection, or mass, of abnormal cells in your brain. Your skull, which encloses your brain, is very rigid, and any growth inside such a restricted space can cause problems. Brain tumors can be cancerous (malignant) or noncancerous (benign). When benign or malignant tumors grow, they can cause the pressure inside your skull to increase, this can cause brain damage, and it can be life-threatening. Early detection and classification of brain tumors is an important research domain in the field of medical imaging and accordingly helps in selecting the most convenient treatment method to save patients life. The application of deep learning approaches in context to improve health diagnosis is providing impactful solutions. According to the World Health Organization (WHO), proper brain tumor diagnosis involves detection, brain tumor location identification, and classification of the tumor on the basis of malignancy, grade, and type.

Dataset

The dataset considered here consists of four classes, including three tumor classes (Pituitary, Glioma and Meningioma) and one class representing normal brain MRI scans. To enhance the diversity and robustness of the dataset, various image augmentation techniques were used. These techniques were applied to the images without altering the labels. Here is a summary of the augmentation methods used:

Salt and Pepper Noise: Introducing random noise by setting pixels to white or black based on a specified intensity.
Histogram Equalization: Applying histogram equalization to enhance the contrast and details in the images.
Rotation: Rotating the images clockwise or counterclockwise by a specified angle.
Brightness Adjustment: Modifying the brightness of the images by adding or subtracting intensity values.
Horizontal and Vertical Flipping: Flipping the images horizontally or vertically to create mirror images.

The clean and augmented dataset can be found at: https://www.kaggle.com/datasets/mohammadhossein77/brain-tumors-dataset/data

## Conclusion

In this notebook we considered a dataset containing (augmented) brain MRI scans divided into four classes: normal MRI scans, pituitary tumor, glioma tumor, and meningiome tumor. In the first part a Deep CNN (containing 4 hidden convolutional layers) was build and tuned. In the second part a pre-trained MobileNet network was used.

The Deep CNN showed better performance reaching an accuracy of about 0.93 on the test set (tha contains about 6500 augmented images). This can be due to the lower size of training data (about 15000 images) and the small size of classes considered (only 4 classes). With a larger dataset and more labels to classify, a better approach could be to fine-tune a pretrained model. 

