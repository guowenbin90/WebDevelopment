### Summary Part 2
In the second part, a Plotly visualization was set up on the back-end inside the routes.py file using Plotly's Python library. 
The Python plotly code is a dictionary of dictionaries. 
The Python dictionary is then converted to a JSON format and sent to the front-end via the render_templates method.

Simultaneously a list of ids are created for the plots. 
This information is also sent to the front-end using the render_template() method.

On the front-end, the ids and visualization code (JSON code) is then used with the Plotly javascript library to render the plots.

In summary:

Python is used to set up a Plotly visualization
An id is created associated with each visualization
The Python Plotly code is converted to JSON
The ids and JSON are sent to the front end (index.html).
The front end then uses the ids, JSON, and JavaScript Plotly library to render the plots.
