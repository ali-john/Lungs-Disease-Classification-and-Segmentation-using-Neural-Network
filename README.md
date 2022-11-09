# Lungs Disease Classification and Segmentation using Neural Network.
----


Close to a billion chest x-rays (CXRs) are taken around the globe every year for diagnosing
different conditions that a patient may be suffering from. This large number of CXRs can lead to
delay in the correct diagnosis and subsequent treatment as the medical professionals may not be
able to keep up with such a large amount of data. Therefore, any kind of automation here can
result in a system that is beneficial to both the medical professionals and the patients.
There are two ways in which a CXR can be useful is:
  - Making a diagnosis of a disease from the CXR (pneumonia, COVID-19, infection etc.)
  - Segmenting out different regions in the CXR (lungs, heart etc.)
  
Using different image processing and deep learning methods both of the above targets will be achieved with good
enough performance so that they become a useful tool for the medical professionals. A timely
diagnosis can result in a saved life.

## Classification of Lung Diseases.
There are 6 different lung classes named Cardiomegaly, pleural effusion, atelactasis, consolidation, edema and no findings. A sample of these diseases is shown:

![image](https://user-images.githubusercontent.com/63426759/200942018-655ee101-64a9-40d0-9689-5ad6a58b0f88.png)

### Model:
Due to outperformance of CNNs in medical images, 7 layer Cnn model is chosen. The architecture of CNN is:


![image](https://user-images.githubusercontent.com/63426759/200942849-4815a3ab-ece0-4e66-b9f1-e2427da8b522.png)

## Output
The model has an accuracy of 67%. The outputs predicted from model is shown below:

![image](https://user-images.githubusercontent.com/63426759/200943636-e4da3cc9-fe86-4bd9-b2d7-eaf17fb70601.png)

![image](https://user-images.githubusercontent.com/63426759/200943815-af7949e3-e3ff-4006-8df9-7931e7e07c19.png)

----
## Segmenting Lung Region
Medical image segmentation, essentially the same as natural image segmentation, refers to the process of extracting the desired object (organ) from a medical image (2D or 3D), which can be done manually, semi-automatically or fully-automatically. The imaging modality of the medical images can be diverse such as CT, MRI, US, PET, X-ray, or hybrid such as PET/CT, depending on the organ to be imaged and the imaging purpose.

Medical image segmentation has an essential role in computer-aided diagnosis systems in different applications. The vast investment and development of medical imaging modalities such as microscopy, dermoscopy, X-ray, ultrasound, computed tomography (CT), magnetic resonance imaging (MRI), and positron emission tomography attract researchers to implement new medical image-processing algorithms. Image segmentation is considered the most essential medical imaging process as it extracts the region of interest (ROI) through a semiautomatic or automatic process. It divides an image into areas based on a specified description, such as segmenting body organs/tissues in the medical applications for border detection, tumor detection/segmentation, and mass detection.

## Model.

Due to wide usage of U-NET in image segmentation specially in medical images, this architecture was adopted. It's architecture is:

![image](https://user-images.githubusercontent.com/63426759/200945163-fd0cb3a1-672f-4b24-95e1-03df3885f772.png)

## Results:

The results of segmentation using U-NET gives close resembalance to given mask.


![image](https://user-images.githubusercontent.com/63426759/200945884-65a6a9cb-ef2b-49d8-8772-44b54678fbcd.png)

![image](https://user-images.githubusercontent.com/63426759/200946091-15904922-d509-4b06-8ed3-af6307c1d8d8.png)
