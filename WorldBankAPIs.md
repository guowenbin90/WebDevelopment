### REST Architecture
REST is a software architecture for the web. 
You don't need to understand how REST works in order to use an API. 
but you will see the term used quite frequently when working with APIs. 
Modern web APIs are often called RESTFul to indicate that they conform to a REST Architecture.

- [REST API Tutorial](https://restfulapi.net/)
- [Wikipedia Article on REST](https://en.wikipedia.org/wiki/Representational_state_transfer)
### World Bank API
Here is the website where the csv files were downloaded for the World Bank web app: 
[World Bank Indicator Data](https://data.worldbank.org/indicator?tab=featured)

And here is the link to the World Bank API documenation: 
[World Bank API Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392-api-documentation)

One tricky aspect of working with the World Bank API is that it only gives back 50 results at a time. 
There is an option called per_page that allows you to return up to 1000 results. However, some queries might have more than 1000 results. That's where the page option comes into play. You'll notice that at the very beginning of the data, there is a variable called page and another one called pages. If page=1 and pages=4, then you'd need to write 4 queries with the option page=1, page=2, page=3 and page=4.
