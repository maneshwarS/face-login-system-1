# Face-login-system
Building a facial recognition system which can be intergrated on a website or an application and can be used by a person to login into a system. Facial recognition is achieved by OpenCV's face_recognition wrapper function and the sigup/login pages are built using HTML and CSS. Database of image encodings are stored in Django's database.
 
## Functioning
On visiting the landing page of the website for the first time, the person will be required to sign-up and the webcam will click images of the person which will be used as a training dataset. The encodings of the images captured will be mapped with the unique username of the person.

During login, the webcam will use OpenCV's face_login wrapping to recognize the person (something like a test image) and will login the person into the system if the encodings of the newly captured image equals the one previously stored in the database.

## Dependencies
* OpenCV
* face_recognition library
* Pillow (PIL: Python Imaging Library)
* HTML, CSS (Creating login/signup pages)
* Django (Creating server responses and storing image database)
