### JavaScript and this Lesson
To build the data dashboard at the end of this lesson, you won't need to write any JavaScript at all. 
That's because you'll use libraries (Bootstrap and Plotly) that take care of the JavaScript for you.

You won't need to get into the details of JavaScript syntax, but it's good to have at least an idea of what is happening under the hood.

### What is JavaScript?
JavaScript is a high level language like Python, PHP, Ruby, and C++. 
It was specifically developed to make the front-end of a web application more dynamic; 
however, you can also use javascript to program the back-end of a website with the JavaScript runtime environment node.
Java and javaScript are two completely different languages that happen to have similar names.
JavaScript syntax, especially for front-end web development, is a bit tricky. 
It's much easier to write front-end JavaScript code using a framework such as jQuery.

### Basic JavaScript Syntax
Here are a few rules to keep in mind when writing JavaScript:

- a line of code ends with a semi-colon ;
- () parenthesis are used when calling a function much like in Python
- {} curly braces surround large chunks of code or are used when initializing dictionaries
- [] square brackets are used for accessing values from arrays or dictionaries much like in Python

Here is an example of a JavaScript function that sums the elements of an array.
```
function addValues(x) {
  var sum_array = 0;
  for (var i=0; i < x.length; i++) {   
    sum_array += x[i];
  }
  return sum_array;
}

addValues([3,4,5,6]);
```
### What is jQuery?
Jquery is a JavaScript library that makes developing the front-end easier. 
JavaScript specifically helps with manipulating html elements. 
The reason we are showing you Jquery is because the Bootstrap library you'll be using depends on Jquery. 
But you won't need to write any Jquery yourself.

Here is a link to the documentation of the core functions in jquery: [jQuery API documentation](https://api.jquery.com/)

Jquery came out in 2006. There are newer JavaScript tools out there like [React](https://reactjs.org/) and [Angular](https://angularjs.org/).

As a data scientist, you probably won't need to use any of these tools. But if you work in a startup environment, you'll most likely hear front-end engineers talking about these tools.

### jQuery Syntax
The jQuery library simplifies JavaScript quite a bit. 
Compare the syntax. 
Compare these two examples from the video for changing the h1 title element when clicking on the image.

This is pure JavaScript code for changing the words in the h1 title element.
```
        function headFunction() {
            document.getElementsByTagName("h1")[0].innerHTML = 
                  "A Photo of a Breathtaking View";
        }
```
This code searches the html document for all h1 tags, grabs the first h1 tag in the array of h1 tags, and then changes the html. 
Note that the above code is only the function. You'd also have to add an onClick action in the image html tag like so:
```
<img src="image.jpg" onclick="headFunction()">
```
The jQuery code is more intuitive. Once the document has loaded, the following code adds an onclick event to the image. 
Once the image is clicked, the h1 tag's text is changed.
```
         $(document).ready(function(){
            $("img").click(function(){
                $("h1").text("A Photo of a Breathtaking View");
            });
        });
```
The dollar sign $ is jQuery syntax that says "grab this element, class or id". 
That part of the syntax should remind you somewhat of CSS. 
For example $("p#first") means find the paragraph with id="first". Or $("#first") would work as well.

Javascript has something called callback function, which can make learning javascript a bit tricky. Callback functions are essentially functions that can be inputs into other functions. In the above code, there is the ready() function that waits for the html document to load. Then there is another function being passed into the ready function. This section function adds an on-click event to an image tag. Then there's another function passed into the click() function, which changes the h1 text.
