# Custom Vision Car Counter
Using Python with OpenCV and a trained model in Azure Custom Vision to detect moving cars on a highway.
The project is based on the Counting Cars project from IBM available here https://github.com/IBM/powerai-counting-cars. Insted of the stand alone PowerAI Software they used in their work, I trained a object detection model in the Azure Custom Vision environment. Cars are detected using the provided API calls to my model.
The code splits the input video into single frames and labels them accordingly. Detected objects are tracked from frame to frame in order to avoid counting them multiple times.

The detection model was trained with 24 manually labeled images from the video and with 24 additional pictures of cars downloaded from the Open Image dataset from Google. 
