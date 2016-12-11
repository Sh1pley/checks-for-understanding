## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  It is an ORM, allows you to use a sort of short hand to execute SQL commands.
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
  Instance methods. Using those attaches a method you can call on, on an instance of that object.
3. What do they allow you to do?
  They allow you to assign other objects to that object and call on them easily as a relationship.
4. What's the difference between agile workflow and waterfall method?
  Agile workflow builds a project with many usable stopping points, allowing you to test functionality as you go becuase 
  you always have a functioning thing at each iteration. Waterfall saves functionality until the project is done.
5. What is the difference between `#new` and `#create`?
  new creates an instance of the object, create makes a new instance and saves it to the database.
6. At a basic level, what does cURL allow you to do?
  visit URLs from your terminal.
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
  students: id, name, (belongs to :teachers by the teacher_id); teachers: id, name, (has many :students with student_ids);
8. Define foreign key, primary key, and schema.
  foreign key is used to relate a database item to another database item. primary key is what a database item is primarily associated by
  and the schema is the set of tables to describe each attribute of your database items.
9. Describe the relationship between a foreign key on one table and a primary key on another table.
  You might assign a foreign key to a table to associate or relate another table through its primary key.
  like a Cars table might have a foreign key of tire_ids that would assign different primary key of a Tire object to that car.
10. What are the parts of an HTTP response?
  status line and status code?
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
  Breaking ActiveRecord requests you repeat into methods in your models. 
  Also breaking your database into more Tables for items you may be repeating alot.


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
  .group - takes a table and will group them into sub categories you can call on later
  .pluck - allows you to pluck or grab a value by specifying the key, from a key , value pair set of data
  .where - easiest search method, has lots of arguments you can pass it to get what you want.
  .not - allows you to disclude items in a search
  .order - allows you to order a returned list of items be a specified attribute.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
  rake db:create_migration - allows you to make/change a table in your database
  rake db:migrate - grabs your migration tables and updates your schema
  rake db:rollback - allows you to go back to the previous schema/database setup you had
4. What can you expect from a group as you begin working together? As you continue working together?
  I think, I would always expect communication. With communication you can always work through issues and stay on task.
5. What two columns does `t.timestamps null: false` create in our database?
  created_on and updated_on
6. What cURL flag can you use to send a `POST` request?
  -d
7. What case does JSON (and JavaScript) use for multi-word variables?
  camelCase?
8. What case does Ruby use for multi-word variables?
  snake_case
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
  schools have many teachers; teachers belong to a school
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
  schools: id, name, (has many :teachers); teachers: id, name, (belongs to :school)
11. Give an example of when you might want to store information besides ids on a join table.
  Im not sure
12. Describe and diagram the relationship between patients and doctors.
  patients have many doctors and doctors have many patients. You would need a join table to associate them:
  could make a table that was a doctor visits table that has patient_id paired to doctor_id at a certain time with a reason.
13. Describe and diagram the relationship between museums and original_paintings.
  musems have many original paintings but original paintins only belong to one museum
14. What are some examples of acceptable values for the parts of an HTTP response?
  Im not sure on this either
15. What types of output do we want to test when we test our controllers?
  Not sure.
16. What could you see in your code that would make you think you might want to create a partial?
  Not sure what a partial is.
17. Why might you use a helper method?
  To improve response time on logic heavy methods
