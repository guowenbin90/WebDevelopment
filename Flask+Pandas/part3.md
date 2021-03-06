### Summary Part 3
In part 3, the code iterated through the data set to create a visualization with multiple lines: one for each country.

The original code for a line chart with a single line was:
```
graph_one = [go.Scatter(
  x = data[0][1],
  y = data[0][2],
  mode = 'lines',
  name = country
)]
```
To make a visualization with multiple lines, graph_one will be a list of line charts. This was accomplished with the following code:
```
graph_one = []
for data_tuple in data:
   graph_one.append(go.Scatter(
   x = data_tuple[1],
   y = data_tuple[2],
   mode = 'lines',
   name = data_tuple[0]
))
```
