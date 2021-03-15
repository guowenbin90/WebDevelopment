### What is an API?
Instead of downloading World Bank data via a csv file, you're going to download the data using the World Bank API.

API is an acronym that stands for application programming interface. 
API’s provide a standardized way for two applications to talk to each other. 
For this project, the applications communicating with each other are the server application where World Bank stores data and your web application.

If you wanted to pull data directly from the World Bank’s server, you’d have to know what database system the World Bank was using. 
You’d also need permission to log in directly to the server, which would be a security risk for the World Bank. 
And if the World Bank ever migrated its data to a new system, you would have to rewrite all of your code again.

The API sits between your web app and the World Bank server. 
And the API allows you to execute code on the World Bank server without getting direct access.

All sorts of companies have public facing APIs including Facebook, Twitter, Google and Pinterest. 
You can pull data from these companies to create your own applications.

In the next section, you’ll get practice using Python to pull data from the World Bank API. 
This will set you up for creating the web app with data from the API instead of using data from a csv file.

### APIs Besides the World Bank
All types of companies have APIs. Some of these APIs are only for internal company use while other APIs help the public consume data. 
A few examples of public APIs include the [Twitter API](https://developer.twitter.com/en/docs), 
the [Google Maps API](https://cloud.google.com/maps-platform/), 
the [Facebook Graph API](https://developers.facebook.com/docs/graph-api), 
and the [US Government Data APIs](https://www.data.gov/developers/apis).

In addition, oftentimes you can find open source libraries or development kits for connecting to an API. 
For example, here is an open source Python development kit for the Facebook Graph API.

Some APIs might be used for pulling data from a database. But other APIs are for adding data to a database. 
For example, you might make an application that automatically tweets the current weather. 
In that case, you would use the Twitter API to post a tweet, which in reality inserts a tweet into Twitter's database.

### Using an API
In the next few parts of the lesson, you'll see how to use the World Bank API. 
This API is relatively straightforward to use. Each API, however, will have a different set up and only allow you to take certain actions. 
In general, you send a request via a web url that specifies the information you want. You receive data back typically in [XML](https://www.w3schools.com/xml/xml_whatis.asp) or JSON(https://www.w3schools.com/xml/xml_whatis.asp).

The XML standard was developed in the 1970s and 1980s and soon became a common way to transfer data over the web. 
JSON was developed in the mid 1990s. Over time, [JSON has increased in popularity relative to XML](https://www.programmableweb.com/news/jsons-eight-year-convergence-xml/2013/12/26) perhaps because JSON is easier to parse.

Some APIs require authentication; essentially the company with the API gives you 'credentials' 
so that they can track how you are using the API and ensure you have the proper permissions.

Some APIs might let you extract data from a database. 
Other APIs might even let you insert data into a database depending on the use case. 
Most APIs include extensive documentation so that you can figure out how to use APIs.

If you ever can’t figure out how to use an API, search online for examples. 
You can search for something like, “Examples for using the World Bank API” or “Examples for using the Facebook API”.

Move on to the next section to see how to use the World Bank API and incorporate it into a web app.
