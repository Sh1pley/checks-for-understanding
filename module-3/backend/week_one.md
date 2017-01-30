## Week One - Module 3 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. What is `json` and why is it important?
  JSON stands for JavaScript Object Notation, it is important because APIs typically respond with JSON 
  or XML. JSON being the easier of the two to work with.
2. What's the difference between `joins` and `includes` in ActiveRecord?
  Joins makes one table out of 2. Includes allows you to access specified attributes without making
  additional queries to the database.
3. What's an API?
  API stands for Application Program Interface, it allows you to access another code bases database through
  http/get requests.
4. How do we test an internal API (in general)?
  You could write request tests, that would test the routes and expect return data in JSON format.
5. What are two different ways to customize your `json`?
  Jbuilder allows you to make javascript views that will format JSON returns
  Serializers will allow you to make a Serializer class that will also format JSON return data.
