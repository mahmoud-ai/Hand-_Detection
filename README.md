# Hand-_Detection
Right and Left Hand Detection Using mediapipe.
Used Libraries :
1-opencv
2-mediapipe


Steps:
Step 1: Import all required libraries
Step 2: Initializing Hands model
Step 3: Hands model process the image and detect hands
Capture the frames continuously from the camera using OpenCV and then Flip the image around y-axis i.e cv2.flip(image, flip code) and Convert BGR image to an RGB image and make predictions using initialized hands model.

Prediction made by the model is saved in the results variable from which we can access landmarks using results.multi_hand_landmarks, results.multi_handedness  respectively and If hands are present in the frame, check for both hands, if yes then put text “Both Hands” on the image else for a single hand, store MessageToDict() function on label variable. If the label is “Left” put text “Left  Hand”  on the image and if label is “Right” put text “Right Hand”  on the image.
