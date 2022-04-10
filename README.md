# SAATHI
This is a model that is aimed at providing lane assistance to visually impaired people & help them navigate in the surroundings
and thus providing them a sense of independence and control while walking through unknown environments. 
 
 It also identifies the objects and gives output in form of speech.

The pipeline of the model used was 

     - Grayscaling the image to reduce computation time( done as we only need intensity gradients).
     
     - Applying Gaussian blurring over the image so that noise from the image is removed.
     
     - Extract the edges in the video frame using canny detection & then segment it to bound.
     
     - Fiding and fitting polynomial curve using polyfit.
     
     - Finding the nearby objects using tiny YOLO object detection.
     
     - Text to speech outputs using pyttsx3.
     
