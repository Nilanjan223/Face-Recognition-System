# Face_Recognition_Mined_Hackathon

Steps to execute the program :

1.Adding of data 

1.1 Adding a single new output:

File - Add_new_employess
Run the 1st Cell i.e. used for initializing the parameters for augmentation.
We have used an albumentation library to transform the experiment data by flipping,changing contrast,brightness etc.
Run the 2nd cell to take the input. Re-run the 2nd cell until the satisfied image is not captured. 
Run the 3rd cell where augmentation of the image is done and these are added to the dataset.

1.2 For Existing data

File - Existing_Data
Run all the cells where
1st cell is used for  initializing the parameters for augmentation
2nd cell is used for generating primary grayscale training data.We have used cascade classifier from OpenCV library to detect faces in gray scale.
3rd cell is used for augmentation of all the primary training data and adding it to the dataset. 


2.Training of Model 

File - face_training
Run the cell.
This cell trains the model and stores the model in the trainer.yml file. 
Algorithm used for training the model is LBPH(Local Binary Pattern Histogram)

3.Face identification 

File - face_recognition
Run this cell.
It will activate the webcam of your device and detect the faces.
We have used the VideoCapture() function from OpenCV to read video footage.
If the faces are detected then their id along with date and time will be added to csv file.
Press Esc to close video capture.
