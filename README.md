#Bear image classifer 
The Bear Image Classifier is a program that predicts a picture of a bear and sends back facts and knowledge about said bears( grizzly, black, teddy, polar, panda) 

# Set up for the backend
Note Node and Python with Pip package manager must be installed as a prerec

Instructions to run the image classifer 

1. Clone or download the repository. 

2. Open the program in CMD and install these pacakges on your machine

```pip install --upgrade pip
pip install tensorflow==2.12.*
pip install Pillow
pip install fastapi
pip install "uvicorn[standard]"
pip install python-multipart
```

3.  Run this command to build the neural network
```commandline
python build-model.py
```

4. Start the middleware by running this command
```
uvicorn main:app --reload
```

If the server started correctly it should look like this below. 
```
INFO: Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to 
INFO: Started reloader process [30708] using WatchFiles 
1/1 [==============================] - 0s 150ms/step 
Predicted class: grizzly 
INFO: Started server process [25568] 
INFO: Waiting for application startup. 
INFO: Application startup complete.
```
#Setup for the Front end
1. Change directory to the view folder by typing in 
```
cd view
``` 
2. Run these following commands to make sure the setup works properly 
```
npm install
npm install axios
```
3. Launch the app by typing
```
npm start
```
This will bring up a website from here click the upload button this will show your file system from here go to the folder where this file is stores and you can use 
images from the bear testing directory provided in these files.
