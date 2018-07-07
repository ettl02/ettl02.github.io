---
layout: post
title:      "Just some Super fun stuff about code"
date:       2018-07-07 18:29:04 +0000
permalink:  just_some_super_fun_stuff_about_code
---



This week I am finishing up object oriented ruby with the final hoorah being my CLI Data Gem Project, which I will finish and post about later next week! 

So far, I have been going through lessons with a surface level understanding. I think I know something but when it comes time to do the lab, I am left totally lost, leaving me having to go back to the lesson to read over and over. But, this time was different. The lessons within Object Architecture - Inheritance and Super clicked with me. 

Here’s what I took from the readings… Inheritance is exactly what it sounds like. Using inheritance allows you to create a class holding all the shared behavior of relationship based classes. The other subclasses or child classes simply inherit the parent attributes using < symbol.

Class Car < Vehicle 

Any change made to that parent class will also change the classes who have inherited from it.   It prevents the need to write tedious code repeatedly for the subclasses.  Aka: DRY (Don’t Repeat Yourself). It is also possible to overwrite  differences between the child and parent class.

Super is a built-in function used similarly to inheritance but has much more (super) powers. If the child class only wants some of the functionality of the parent class, then the child class simply re-defines the method they want to run from the parent class and writes the keyword #super underneath. Then, any additional code written, will be unique to the child class. 

For instance: 


```
class User
  def log_in
    @logged_in = true
  end
end


class Student < User
  def log_in
    super
    @in_class = true
  end
end
```
 
Super has way more uses than this. Super can be used on the initialize method, with or without arguments that are sent to the super class. But this article can explain it way better than I can 😊 https://launchschool.com/books/oo_ruby/read/inheritance


Ok, now it’s time to get back to coding. 

