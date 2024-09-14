OPEN CV IMAGES PYTHON LIBRARY CODE:
import cv2
# Initialize the webcam
cap = cv2.VideoCapture(0)
while True:
# Capture frame-by-frame
ret, frame = cap.read()
# Display the resulting frame
cv2.imshow('Webcam Video', frame)
# Break the loop on 'q' key press
if cv2.waitKey(1) & 0xFF == ord('q'):
break#
Release the capture and close the windowcap.release()
cv2.destroyAllWindows()
