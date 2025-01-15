# Face_Recognition_System
The facial recognition system will identify a person with the help of his/her facial features. The facial recognition system proves to be  the easiest method to identify a person.

Line 1-9: We are importing the required libraries.
Line 11-12: Defining the Flask App.
Line 14-15: We are defining a constant ‘nimgs‘ which defines how many images to capture for each user while registering.
Line 17-18: Getting today’s date to use in the program ahead.
Line 21-22: Loading the ‘haarcascade_frontalface_default.xml‘ HaarCascade file to detect faces.
Line 25-34: Checking if the required folders are in place or not, If not create them. Also, create today’s attendance file if it’s not present in the Attendance folder.
totalreg(): A function that counts the total number of registered users.
extract_faces(): A function that extracts the face from an image. It uses the HaarCascade file we loaded above.
identify_face(): A function that identifies the faces in the given image using the trained KNN model.
train_model(): A function that trains the KNN model on all the faces available in the faces folder.
extract_attendance(): A function that extracts information from today’s attendance file in the attendance folder.
add_attendance(): A function that adds the Attendance of a specific user in today’s Attendance file.
Routing Functions:

home(): Our main page routing function.
start(): Our main function that will take attendance when we click on the Take Attendance Button.
add(): Function to add a new user.
The last 2 lines are to run the Flask App.
