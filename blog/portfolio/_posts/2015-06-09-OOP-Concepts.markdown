---
layout: post
title:  "OOP Concepts"
date:   2015-9-06 11:00:34
categories: technical
---

#Variable Scope#

Variable scope is an important tool in any language and allows some variables to be applicable everywhere in a project or just used for an iterator in a single if statement.

#Constant#

Constants are designated as:

{% highlight ruby %}
VARIABLE = 5
{% endhighlight %}

Constants are just as they sound. They are set at the beginning of a program and are meant to be unchanged. Ruby itself doesn't mind if you change it to something else but it will give you a warning as that isn't what they are designed to do.

#Global#

Global variables ar written:

{% highlight ruby %}
$global = 5
{% endhighlight %}

Global variables are designed to be across all types of classes or methods and really anywhere in your program

#Class Variable#

Class variables are written:

{% highlight ruby %}
@@class_variable = 5
{% endhighlight %}

Class variables stay the same through all instances of the class and are usefull for things that don't ever change for your class.

#Instance Variable#

Instance variables are written:

{% highlight ruby %}
@instance_variable = 5
{% endhighlight %}

Instance variables are re-used everytime you create a new instance of the class so if your class is a person the person can be different every time.

#Local Variable#

Local variables don't have any special designation and are useful for iteration. Local variables are only good for that particular block of code.