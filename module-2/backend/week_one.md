## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
  Get, Post, Redirect, Render, Put
2. What is Sinatra?
  A local hosting service to test http functionality.
4. What is MVC?
  Models, views, controllers
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  So that other coders/people can look in to our app and make sense of it.
6. What types of variables are accessible in our view templates without explicitly passing them?
  instance variables, in that specific block
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    ** @name = 'Mr. Ed'
    ** @count = 1 **
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
  see above
9. What's the purpose of ERB?
  to provide an html file that can process ruby code in interpolation <% %>
10. Why do I need a development AND test database?
  So you can specify what you want to test and not have to test through all of the data in the dev database
11. What's responsive design?
  A front end design that responds quickly to requests
12. What is CRUD and why is it important?
  Create, Review, Update, Delete : provides a structure for basic web database interaction
13. What does HTTP stand for? 
  Hyper text transfer protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  <%= and <% brackets. The bracket with the = sign included will output the results to the html page
15. What's an ORM?
  Object Relational Mapper
16. What's the most commonly used ORM?
  not sure
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
  See all - Get/Render
  See one - Get/Render
  Form to add - Get/Render
  Submit change - Post/Redirect
  Form to update - Get/Render
  Submit update - Post/Redirect
  Delete - Delete
18. What's a migration? formatting a database to accept info specified 
19. When you create a migration, does it automatically modify your database?
  no
20. How does a model relate to a database? 
  it handles logic in code to manipulate requests or changes to the database
21. What's the difference between agile workflow and waterfall method?
  Agile has something thats functional between each iteration; waterfall saves functionality until the end
22. What is the difference between `#new` and `#create`?
  new makes an instance
  create makes and instance and saves it to the database
