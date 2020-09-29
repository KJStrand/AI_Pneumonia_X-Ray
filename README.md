# Pneumonia Detection from Chest X-Rays

<p align="center">
  <img src="InputImage.png" />
</p>

**Summary**

Apply a convolutional neural network to detect Pneumonia in X-Ray images.

Part 1) Exploratory Data Analysis of NIH X-Ray dataset.
***EDA.ipynb***

Part 2) Build and train model.
***Train_model.ipynb***

Part 3) Load and execute model for inference on test data.
***Inference.ipynb***

**Intended Use:**
This algorithm is intended to be used as an early screening aide to detect Pneumonia for further referral to radiologist. 

**Indications for Use:**
- Patient Age: 10 to 75
- Patient Gender: M and F
- Chest X-Ray with view positions: AP and PA

Clinical Setting:
The algorithm is intended for integration into the workflow of diagnostic clinics. This is not an emergency detection scenario, so x-ray images may be sent to a remote server for processing. DICOM format following HIPAA rules must be used for all X-Ray images. Each X-Ray DICOM metadata is first verified for correct patient information (see *DICOM Checking Steps*). If the X-Ray passes the DICOM verification step, the image is then pre-processed and input to the machine learning algorithm, yielding a prediction. After the prediction is complete, the result is sent to a radiologist. The radiologist will give the final diagnosis based on their own independent analysis of the image and the prediction given by the algorithm.

Additional details included in FDA Device submission: ***FDA_Submission.pdf***

Project completed as part of Udacity AI for Healthcare course (2020).
