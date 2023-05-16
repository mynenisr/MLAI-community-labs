# MLAI-community-labs
Labs that explain complex ML/AI ideas simply with code.

# Training a ML box detector
Using Azure custom vision and cognitive service, we are training a model to detect boxes, once a box is detected it will 
notify the user along with an image showing where the box is. 

# Requirements
- [Azure computer vision](https://github.com/Azure/azure-sdk-for-python)
- [Azure custom vision](https://github.com/Azure/azure-sdk-for-python)
- [Azure storage](https://github.com/Azure/azure-sdk-for-python)
- [Msrest](https://github.com/Azure/msrest-for-python)
- [OpenCV](https://github.com/opencv/opencv-python)
- [Twilio](https://github.com/twilio/twilio-python/)

# In a Nutshell
- Install all the required modules from requirements.txt `pip install -r requirements.txt`
- Add all the following required variables in a .env file
```env
CONNECTION_STRING = Storage connection string
SOURCE = 'usb' or path to any .mp4 file
TIME_DELAY = Specifies frame capture interval in seconds
MANUAL_MODE = Set 0 for auto and 1 for manual mode
PREDICTION_KEY = Azure cognitive service key
TRAINING_KEY = Azure cognitive service key here as well
PROJECT_ID = Custom vision project id
TWILIO_ACCOUNT_SID = Account SID from twilio
TWILIO_AUTH_TOKEN = Auth Toekn from twilio
TWILIO_PHONE_NUMBER = Twilio phone number
```
- The source can be direct video stream from a camera(USB), or from a .mp4 file.
- Time delay sets the time threshold to capture frames from the video.
- You can choose from two modes, manual(1) or auto(0).
- Finally, `py edge_to_blob.py`

# Quick tutorial

https://github.com/initmahesh/MLAI-community-labs/assets/62789637/f24d80e0-102a-4b04-a4a6-b35c37ac4ac6

