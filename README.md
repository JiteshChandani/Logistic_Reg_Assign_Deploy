# Logistic Regression

Deploying the Affair Dataset which comes from Statsmodel ML problem using flask. It was derived from a survey of women in 1974 by Redbook magazine, in which married women were asked about their participation in extramarital
affairs. More information about the study is available in a 1978 paper from the Journal of Political Economy.

We've decided to treat this as a classification problem by creating a new binary
variable affair (did the woman have at least one affair?) and trying to
predict the classification for each woman.

# 1. Train ML model

Machine Learning model is build using Logistic Regression technique in order to predict the Extra Marital Affair.

# 2. Create a web app using Flask

I have defined the app routes and completing the main.py file, and created a index.html which will serve as the home page, which contains all the field required to run the model.

![image](https://user-images.githubusercontent.com/75501488/139122973-35412494-eb41-4433-a33a-58f7b5fd608e.png)

# 3. Commit the code to GitHub

Now create some of the required files for deployement and then commit all the files to GitHub.

Most important thing is to create a Procfile and requirement.txt, which handles the configuration part in order to deploy the model into heroku server. 
web: gunicorn is the fixed command, after that the first parameter is main.py file i.e the file which will be executed first. Provide the first parameter without the file extension. 
Second parameter is the flask app name. Requirements consists of all the libraries that has to get installed in heroku environment.

# 4. Connect GitHub to Heroku

Heroku is a multi-language cloud application platform that enables developers to deploy, scale, and manage their applications. Heroku is elegant, flexible, and easy to use, offering developers the simplest path to getting their apps to market.
Heroku gives the direct option to connect with GitHub and deploy the code.

![image](https://user-images.githubusercontent.com/75501488/138836204-bdfc04d7-1a20-494f-b5d7-23fa5ef70999.png)

# 5. Deploy the model

After successful deployment, app will be created. Check out the web-app: https://affairprediction.herokuapp.com/
