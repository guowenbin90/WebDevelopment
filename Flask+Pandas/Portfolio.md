### Portfolio Exercise: Deploy a Data Dashboard
Personal portfolios are an excellent way to demonstrate your knowledge and creativity. In fact, they are little by little becoming a must-have for people working in the tech industry. In this portfolio building exercise, you will create a data dashboard using Bootstrap, Plotly, Flask and Heroku.

Note that a portfolio exercise like this is not reviewed. So you will not submit your work on this, and you do not need to complete this assignment in order to graduate.

Your main job will be to write Python code that reads in data, cleans the data, and then uses the data to make Plotly visualizations. This is your opportunity to show off your Python coding ability and visualization encoding skills.

In the next part of the lesson, you'll find a workspace where you can develop the web app. Note that there is also an optional advanced version of the project where you're encouraged to pull data from an API. You'll see in this lesson that there are a few sections with "[advanced version]" in the title. If you'd like to do the advanced version, then you'll want to go through this entire lesson before starting to develop your app.

### General Instructions
Develop and deploy a data dashboard. The Web Development lesson has all of the information you need. If you are new to web development, you might have to go back to the concepts and rewatch some of the videos. The "deployment" parts of the lesson should be especially helpful. The video in that part of the lesson shows how to deploy a web app to Heroku. And the associated exercise has a complete, functioning web app with visualizations.

Most of the work will involve:

Wrangling your chosen data set to get the data in the format you want
Writing Python code to read in the data set and set up Plotly plots
Tweaking HTML so that the website has the design and information that you want.
We are providing a template that uses the Bootstrap library and Flask framework. The template is the same one used to build the app in the course except the name of the app has been changed. In the template, everything has the generic name "myapp" instead of "worldbankapp". The template is set up so that you can use pandas for loading the data and Python to create the dictionaries needed for plotly.

You'll only need to modify the following files:

wrangle_data.py
index.html
Although the front-end is already set up for you, you should change the links and titles in index.html. If you want to add more visualizations or remove visualizations, you'll need to adjust the front-end code in index.html accordingly. That will involve adding or removing rows and columns in the HTML file.

For deployment, you can use a back-end service like Heroku.

### How to Build the App
You'll find a workspace in the next part of the lesson. The workspace already contains the template code with a working web app. The web app has a back-end and front-end. Recall that you can run the web app from the workspace:

To run the app from the workspace, open a terminal and type env | grep WORK. Note the WORKSPACEDOMAIN and WORKSPACEID. To start the web app, type python myapp.py.

You can open a new browser window and go to the address: http://WORKSPACESPACEID-3001.WORKSPACEDOMAIN replacing WORKSPACEID and WORKSPACEDOMAIN with your values.

However, there is no data for the visualizations. You'll need to write a Python script that reads in the data files of your choosing and sets up the plots for Plotly. The process will be exactly the same as the one presented in the web development course.

If you need to upload any files to the workspace, you can do so by clicking on the plus (+) sign and choosing "add file" or "add folder".

The template code is also available on GitHub as part of the data scientist nanodegree term 2 repo.

Test your app in the workspace to make sure that everything is working. You'll see that if you start the app without modifying any of the code, the app currently works.

You should also save your work to a GitHub or GitLab repository so that you can use your code as part of your professional portfolio.

Once you're ready to deploy the app, don't forget to remove the app.run() line of code in the myapp.py file (In the web development lesson, myapp.py was called worldbank.py). You'll need to add a Procfile and requirements.txt file as well. Follow the instructions in the web development lesson to learn how to deploy the app from the classroom. And always comment your code :-)!

Also, at the end of this page you're reading, you'll find information about a more advanced version of the data dashboard that you can build.

### Steps
Here is a reminder of the steps you'll need to do:

find a data set or a few data sets that you're interested in
explore and clean the data set
put the data into a csv file or files - you can use pandas or spreadsheet software to do this
upload your data sets to the correct folder
write a Python script to read in the data set and set up the Plotly visualizations
set up a virtual environment and install the necessary libraries to run your app
run your web app locally to make sure that everything works
deploy the app to Heroku or some other back-end service
Where to Build the Web App
We are providing a workspace containing a web app template. You can use this template to build and deploy your web app within the classroom.

The classroom has an Ubuntu Linux environment. Developing the app locally on macOS should be very similar. On a Windows machine, the commands are slightly different and you'll need to use the command prompt. This link contains a comparison of MS-DOS vs Linux commands.

To install the Heroku command line interface on a Windows machine, follow the instructions here on the Heroku website.

Advanced Version of the Exercise
If you'd like an extra challenge, consider using an API to obtain your data. API stands for Application Programming Interface. An API provides a convenient way for two applications to communicate with each other. To be more concrete you can pull data directly from the World Bank API, clean the data in the back-end using pandas, and then display the results on your front-end. This would be instead of using a csv file for your data.

The benefit is that if the data ever changes, your web app will automatically have the correct data. Many companies provide APIs for accessing their data including Facebook, Twitter, Google among others. As an example, here is an API for pulling data about DVDs, movies, books, and games.

After the workspace, you'll find a set of concepts that explain how to use the World Bank API. Go through that material if you'd like an extra challenge for building your web app.
