# covid_vs_non-covid
Binary Classification of ct scan images of covid-19 and non covid images

-Distinguishing COVID-19 from normal lung or other lung diseases, such as lungs cancer, bacterial pneumonia, may be a major hurdle in controlling the current pandemic.

-Manual radiologist interpretation of chest CT for recognizing COVID-19 by its characteristic patterns that include peripheral ground-glass opacities, but unfortunately this measure often has low specificity.

-Therefore, an efficient classification method using neural network and transfer learning can give us better accuracy in classification of CT scan.


# visulization of covid and non-covid
-From the image we can see that covid-19 ct scan has round glass opacities which is not seen in the non- covid patient ct.

-These feature can be used to classify the images but with help of  convolution neural network (CNN) which are specially designed for feature detection can give better classification results.  


![image](https://user-images.githubusercontent.com/58631474/123285252-82848e00-d52a-11eb-91b5-fef6bc8c7b53.png)

# image tranformation or data augmentation

-Data Augmentation is very important to regularize our network and increase the size of our training set.

-Data transformation techniques (rotation, flip, crop, etc…) that can change the images pixel values and bring more information from the images for better classification.

-This forces the model to be more flexible with the large variation of object inside the image, regarding less of position, orientation, size and color.

![image](https://user-images.githubusercontent.com/58631474/123285648-db542680-d52a-11eb-9981-7d13888a4de9.png)

# division of data into training validation and testing

The dataset is divided into training validation and testing.
-Number of images for training : 1488

-Number of images for validation : 496

-Number of images for testing :496

# class imabalance

![image](https://user-images.githubusercontent.com/58631474/123286006-279f6680-d52b-11eb-8746-10959feedfc9.png)
![image](https://user-images.githubusercontent.com/58631474/123286045-30903800-d52b-11eb-8247-f8aa469ed178.png)

# model architecture

-The configuration of dense layers was as follows: three fully connected layers of 16, 32 and 400 neurons, respectively, combined with 0.5 dropout using rectified linear unit activations with batch normalization![image](https://user-images.githubusercontent.com/58631474/123286162-4e5d9d00-d52b-11eb-8486-87623c5db4b8.png)

![image](https://user-images.githubusercontent.com/58631474/123286249-62090380-d52b-11eb-80b2-46f4569b18e5.png)

# Results
-
-Compared with results from both the model the model with  20 epochs has accuracy of 67% whereas the model with 40 epochs has accuracy of 73%.
