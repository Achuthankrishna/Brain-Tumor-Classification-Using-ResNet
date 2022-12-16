# BrainTumorClassificationUsingResNet
The repository consists of Brain Tumor classification using ResNet50 and ResNet150V2. The images were cropped using RICAP and were fed into the model.

RICAP was done on the input - Taking centre of mass of the image intensity and defining region of interest to be 256 x 256. Rescaling was done on the input image from varied sizes to standard MRI Image size. We thank dataset contriutors [Kaggle] for providing with the dataset of MRI scans.

4 Models were trained on :
a) CNN - 6 CNN model with increasing filter sizes along with Dropout and Batchnorm
b) MobileNet - Adam optimizer with a Lr of 1e-3
c) ResNet50 - 3 Dense Layers
d) ResNet152V2 - 3 Dense Layers

Running Instructions :
- For Resizing and Cropping : Open Cropping.Ipynb. Remember to include your dataset path and ensure you read your image dataset size before usage of the code. Install pyrodynamics library and Simple ITK library as is was used to extract image COM.
- Remeber to install cv2 on your local system (CUDA) 
- Ensure you resize the images in Meningioma and Pituitary tumors before cropping 

