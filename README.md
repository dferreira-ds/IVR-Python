# IVR using Python, Twilio and Ngrok
This repository shows how to create a simple IVR using Python and Twilio

### Step one

The first thing is you need to make sure to install the Twilio library and Flask framework.

1. To install Twilio library, please follow this https://www.twilio.com/docs/libraries/python.
2. To install the Flask framework, please use this https://pypi.org/project/Flask/.

### Step two

Save the ivr_test.py script on your computer. From this example, you will notice that you get different replies depending on your answer, see the "if" conditional. You may add the `<Dial>` verb in one of the conditionals if you want the call to be routed to another phone number, more info can be found here https://www.twilio.com/docs/voice/twiml/dial.

### Step three

Then, if you are running windows or mac, you need to open the command prompt or the terminal, respectively, and navigate to where you saved the file. 

For windows, you need to run the following:
```
set FLASK_APP=ivr_test.py
flask run
```
  
For mac:
```
export FLASK_APP=ivr_test.py
flask run
```
### Step four
  
Up to this point, you have made your web application available in your localhost. Now, you need to make it public on internet. If you do not have a server available at the moment, I would recommend to check out ngrok. This application allows you to host your web app on the internet for 2 hours (for free accounts) so you can test your application. In this Twilio blog https://www.twilio.com/blog/2013/10/test-your-webhooks-locally-with-ngrok.html you will be able to see how you can use ngrok and how to configure your webhook on your Twilio console.
