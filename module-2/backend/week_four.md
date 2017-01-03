## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
  A cookie is a stored bit of data from your visit in a web session. It could include files you had to download to load a page, or information you subbmitted to the site.

* What’s the difference between a session and a cookie?
  A cookie is in mostly plain text and readable, where a session has been hashed/encrypted for safety. Session info is more safe to utilize within a web app.

* What’s a flash and when do you want to use flashes?
  A flash is a notification to the user when something goes well or bad, It is an internal hash data set that you can specify the keys to save data in the value to notify a user.

* Why do people say “HTTP is stateless”?
  It is said to be 'stateless' because it remembers nothing between instances. There is no state kept at the server level.

* What’s authentication? Explain.
  Authentication is setting up individual users in a web app, so that you know who is accessing the app and can tailor the experience to.

* What’s the difference between authentication and authorization?
  Authentication is knowing who is accessing; Authorization is limiting them to what they can access within your app.

* What’s a before filter?
  Also called a before_action. Requires a method to be called before each specified action if used with only: or before all actions if not specified.

* How do we keep track of a user once they’ve logged in?
  Adding their info to the sessions hash, as a params[:session][:user_id]

* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
  Namespacing can be used for admin type access, or a type of route where specific authorization may be needed, and is outside of the regular routes or has different access to the regular routes.
  Nesting, is when one model within a route would require another model. Like a cars route would probably be required to specify a driver. ex: cars/2/drivers/1

* At a high level, what tools can you use to implement authorization? How would you use them?
  Bcrypt. Allows encrypted passwords and user authentication in the background of your app. It allows for more security.

* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
  An enum is a way to make an integer in a data table correspond to a special named method. like a 0,1,2 for default, admin, guest users.

* What are some strategies you can use to keep your views DRY?
  helper methods, and partials.
