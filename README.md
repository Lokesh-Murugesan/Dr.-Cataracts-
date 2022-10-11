# Dr.Cataracts
An Image Processing project developed using a pre-trained VGG-19 Deep Convolutional Neural Network model. The objective is to classify whether the eyeball has cataract or not with the help of eye fundus images.

### ABSTRACT:
Humans, being visually oriented, witness the happenings in the surroundings with the help of eyes. In the current scenario, blindness, and visual impairment has become a major and ubiquitous health problem. Although new technologies are rapidly progressing, visual impairment remains a noteworthy problem for worldwide healthcare systems. One of such problems is Cataract. Cataracts causing poor vision may also result in an increased risk of falling and depression. Earlier, it was usual among old age people, but now childhood cataract has become an important cause of blindness and severe visual impairment in children. Existing studies have been done mostly on Fundus image datasets for automatic detection of cataract and grading using a predefined feature set. The challenge is to detect cataract using the normal lens images at an early stage thus allowing people to test for cataract themselves. This would rather ensure that people belonging to remote areas need not reach out to ophthalmologists, just to check whether the person is facing a cataract problem or not. This paper uses CNN models taking normal lens image input for detection of cataract problems.

### ABOUT THE DATASET:
Ocular Disease Intelligent Recognition (ODIR) is a structured ophthalmic database of 5,000 patients with age, color fundus photographs from left and right eyes and doctors' diagnostic keywords from doctors. This dataset is meant to represent ‘‘real-life’’ set of patient information collected by Shanggong Medical Technology Co., Ltd. from different hospitals/medical centers in China. In these institutions, fundus images are captured by various cameras in the market, such as Canon, Zeiss and Kowa, resulting into varied image resolutions. Annotations were labeled by trained human readers with quality control management. They classify patient into eight labels including:
•	Normal (N),
•	Diabetes (D),
•	Glaucoma (G),
•	Cataract (C),
•	Age related Macular Degeneration (A),
•	Hypertension (H),
•	Pathological Myopia (M),
•	Other diseases/abnormalities (O).

![image](https://user-images.githubusercontent.com/79091565/195017913-13275b4e-826d-4b77-bd2c-211894bc32b2.png)

### WORKFLOW:
The implementation methodology begins from a collection of good image dataset for both the classes namely cataract and normal eye. Image preprocessing is done involving 2 steps, resizing the images to a specific size and cropping the image borders. Due to a very high fluctuation in the size of images, all images need to be downsized to a common size of width 50 pixels and height 50 pixels. A model or a binary classifier is created in order to make predictions. This model is trained by feeding a training dataset to the model. The model is supposed to predict whether the image belongs to class cataract or non-cataract. The images of the data set used for testing is not the same as that used for training as the model may memorize the unimportant features of the training images. This issue is known as over fitting, and to avoid it we keep a portion of our dataset out of the training procedure. After the testing phase, the model is ready to predict for new images.

### SAMPLE OUTPUT:

![image](https://user-images.githubusercontent.com/79091565/195018458-cbd6cfd8-3a29-468e-ae06-01b8b08fd816.png)

### RESULTS AND INTERPRETATIONS:
![image](https://user-images.githubusercontent.com/79091565/195018550-a2469b65-655b-49f4-a97c-2dd42fdb9215.png)

From the above classification report, we can infer that the VGG-19 model is performed well with the accuracy of 0.99. The precision, recall and f1-score are also having better values.
