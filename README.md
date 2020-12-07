# image-microservice
This microservice is used to get and post images. Images from a local computer are uploaded to by the micro service using the post method. Then they are later retrieved from the API data base using the get method.
A major issue I faced was having the api run on AWS and this was becuase I was using Tkinter library for uploading images from a computer.

# Steps to run it locally
Navigate into the local subfolder and run the uvicorn command.
 - uvicorn app.main:app --reload
Get the url link and run it in POSTMAN. 
 - POST Method - http://127.0.0.1:8000
 - GET  Method - http://127.0.0.1:8000/{id}
 Use the image id of an image that was already posted.

# Different Endpoints:
The api has 2 endpoints:
Post Method:
 - http://127.0.0.1:8000
Get  Method:
 - http://127.0.0.1:8000/{id}
