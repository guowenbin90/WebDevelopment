### Summary Part 4
In the last part, three more visualizations were added to the wrangling Python module. The wrangling included reading in the data, cleaning the data, and preparing the Plotly code. Each visualization's code was appended to a list called figures. These visualizations were then imported into the routes.py file. This figures list was sent from the back end to the front end via the render_template method. A list of ids were also sent from the back end to the front end.

Then on the front end (index.html), a div was created for each visualization's id. And with help from the JavaScript Plotly library, each visualization was rendered inside appropriate div.

### Beyond a CSV file
Besides storing data in a local csv file (or text, json, etc.), you could also store the data in a database such as a SQL database.

The database could be local to your website meaning that the database file is stored on the same server as your website; alternatively, the database could be stored somewhere else like on a separate database server or with a cloud service like Amazon AWS.

Using a database with your web app goes beyond the scope of this introduction to web development, here are a few resources for using databases with Flask apps:

Tutorial - Using Databases with Flask
SQL Alchemy- a Python toolkit for working with SQL
Flask SQLAlchemy - a Flask library for using SQLAlchemy with Flask
