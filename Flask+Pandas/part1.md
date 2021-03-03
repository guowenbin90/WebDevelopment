### Summary Part 1
The purpose of this section is to give you an idea of how the final web app works in terms of 
passing information back and forth between the back end and front end. 
The web template you'll be using at the end of the lesson will already provide the code 
for sharing information between the back and front ends. 
Your task will be to wrangle data and set up the plotly visualizations using Python. 
But it's important to get a sense for how the web app works.

In the video above, the data set was sent from the back end to the front end. 
This was accomplished by including a variable in the render_template() function like so:

```
data = data_wrangling()

@app.route('/')
@app.route('/index')
def index():
   return render_template('index.html', data_set = data)
```
What this code does is to first load the data using the data_wrangling function from wrangling.py. 
This data gets stored in a variable called data.

In render_template, that data is sent to the front end via a variable called data_set. 
Now the data is available to the front_end in the data_set variable.

In the index.html file, you can access the data_set variable using the following syntax:
```
{{ data_set }}
You can do this because Flask comes with a template engine called Jinja. Jinja also allows you to put control flow statements in your html using the following syntax:

{% for tuple in data_set %}
  <p>{{tuple}}</p>
{% end_for %}
```
The logic is:

Wrangle data in a file (aka Python module). In this case, the file is called wrangling.py. The wrangling.py has a function that returns the clean data.
Execute this function in routes.py to get the data in routes.py
Pass the data to the front-end (index.html file) using the render_template method.
Inside of index.html, you can access the data variable with the squiggly bracket syntax {{ }}
