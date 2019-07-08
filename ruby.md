# Ruby Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.


#### 1. What is a method in Ruby? How is it different or similar to functions in JavaScript?
methods in Ruby are all functions since everything in Ruby is an object. All methods are functions but not all functions are methods. Methods are specific to only that class whereas functions can be used generally.

#### 2. What does it mean that a class inherits from another class? Try to explain Ruby inheritance. 


[Your Answer]
Inheritance is when a class inherits properties or methods from a parent class above. The parent class becomes a template for the child class but the child class can then be modified further by overriding existing 
properties or methods listed in the parent class.

[Googled Answer]
Inheritance provides the concept of “reusability”, i.e. If a programmer wants to create a new class and there is a class that already includes some of the code that programmer wants, then he or she can derive a new
class from the existing class. By doing this, it increases the reuse of the fields and methods of the existing class without creating extra code.

#### 3. What is rspec and what is the general process for writing tests in RSpec?

//Your Answer
rspec is a testing framework for Ruby. The general process is BDD (behavior driven development) where you write a test for a function you want your program to have and then implement it.

//Googled Answer
RSpec is a 'Domain Specific Language' (DSL) testing tool written in Ruby to test Ruby code.[4] It is a behavior-driven development (BDD) framework which is extensively used in production applications. 
The basic idea behind this concept is that of Test Driven Development (TDD) where the tests are written first and the development is based on writing just enough code that will fulfill those tests followed 
by refactoring.

#### 4. Name three possible non-inheritance relationships between ruby objects? 

//Your Answer
has many
belongs to
has many of each other

//Googled Answer
Three important relationships in Ruby are known as ‘belongs to…’, ‘has many…’, and “has many of each other”. The ‘belongs to’ and ‘has many’ relationships are considered to be the inverse of one another.
If one class belongs to another, it will have the name of the class that it belongs to listed under attr_accessor. Then set the writer method to equal an instance of the class it belongs to. 
Typically, a film will have just one director and therefore belongs to that director.
If a class has many of another, it will have an array of the second class in its initialize method. To add song instances to that array, use an instance method called “add_<element_name>”on the initial class
(the one that has many of the other). For this example, we are looking at the relationship between directors and films. Typically, a director will have multiple films.
This relationship is slightly more complicated to express in code, but draws on the previous two relationships. Both of the previous programatic language has to be built into both classes. For this example, 
we are looking at the relationship between films and actors. Typically, actors have many films that they are in, and films have many actors in them.

#### 5. What do we call the #{} convention used below? What is it accomplishing?
String interpolation. It lets you easily read the output by inputting variables directly inside a string.
```ruby
x = 1022
puts "I am printing a random number #{x}"
```

#### 6. How do you feel about testing right now? What potential pros/cons/barriers/advantages do you see to implementing BDD in your own code?

//Your Answer
I feel the same as most other people. It definitely makes coding take much longer and I don't have the experience to say otherwise. I can only trust that what Matt said is true that testing actually does
make everything faster in the long run. I think it's important if there are jobs solely dedicated to testing.
Pros: Sets a straight path so you can't get distracted with ice box addons
Cons: Takes a lot of time and need to learn the testing framework
Barriers: Takes a lot of time. I'm always tempted to just always rush into the coding
Advantages: Would want to learn it just for the resume addition

//Googled Answer
Pros:
Forces code to be modular in order to be tested
Code easier to refactor and maintain
Helps programmers easily understand the code

Cons:
Takes a lot of extra time upfront to code
Requires whole team to buy into testing
Test suite itself needs to be maintained, refactored
Needs experience to do it well

#### 7. What is an instance variable in Ruby? How is it different from a normal, local variable?

//Your Answer
An instance variable in Ruby is a variable that is linked to that specific object's scope. A local variable can be accessed by all objects, but an instance variable can only be accessed by that specific 
object.

//Googled Answer
An instance variable has a name beginning with @, and its scope is confined to whatever object self refers to. Two different objects, even if they belong to the same class, are allowed to have different 
values for their instance variables. From outside the object, instance variables cannot be altered or even observed (i.e., ruby's instance variables are never public)

#### 8. Ruby has a great community and tons of free resources to help you learn. Here is the long list of great resources: https://www.ruby-lang.org/en/documentation/. Below are a few popular ones:
- Interactive Ruby tutorial (http://tryruby.org/levels/1/challenges/0)
- Why's (poignant) Guide to Ruby: comics, anecdotes, and microscopic canaries (http://poignant.guide/book/chapter-1.html)
- Ruby in 20 min (https://www.ruby-lang.org/en/documentation/quickstart/)


Choose one of these resources and go through the material (not for hours, only looking for around 10min of your time) then come back here and list a few new things you learned about Ruby.

Commas are not allowed in numbers, but underscores are. So if you feel the need to mark your thousands so the numbers are more readable, use an underscore.
population = 12_000_000_000

Both exclamation marks and question marks may be used in method names.

Think of the at symbol as meaning attribute.

A range is two values surrounded by parentheses and separated by an ellipsis (in the form of two or three dots).
Normally, only two dots are used. If a third dot is used, the last value in the range is excluded.