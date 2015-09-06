---
layout: post
title:  "Ruby Classes"
date:   2015-9-06 10:58:34
categories: technical
---

#Instance Variables#

Instance variables are normal varables that you use every except that they can be used across methods. In the class above called address the method "title" takes an argument name. This name is currently a local variable and will return an error. On the next line, however, we set the instance varable @name equal to name. This means that we can now use @name in order to call the variable from other places in the class. It doesn't have to be the same name as the local variable it just makes it easy this way!

#Instance Methods#

This code excerpt is from railstips.org

{% highlight ruby %}
class Foo
  def baz
    puts 'instance method'
  end
end
{% endhighlight %}

Here we just have a class called 'Foo' and inside of this is a method called 'baz'. This method just puts "instance method" because Foo.new.baz calls it as an instance. The main part that defines an instance method is that you have create a new "instance" in order to use them.<