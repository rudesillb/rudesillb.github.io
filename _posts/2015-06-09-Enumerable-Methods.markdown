---
layout: post
title:  "Enumerable Methods"
date:   2015-9-06 10:56:34
categories: technical
---

#Enumerables#

Many times in other coding languages you find yourself spending time on the logic behind what you are try to do. Ruby trys to make this whole process easier by providing the methods in the Enumerable Module. These methods make it easy to "do" things to larger sets of data objects. Everything in the module can be completed with "normal" coding logic but enumerables make them easier and more compact.

#Map#

The Map enumerable is inherently non-destructive and is a helpful method when modifying arrays. Lets say we want to modify the array: numbers

{% highlight ruby %}
numbers = [5,8,23,42,61]
{% endhighlight %}

We can use our enumberable map but since it's non-destructive we need to use another array and set it equal to numbers and our .map method.

{% highlight ruby %}
numbers_new = numbers.map {}
{% endhighlight %}

So now we have a new array and our old array is ready for us to .map it! In the curly brackets we need to specify a variable to use as an instance of how to modify array. Since the array only has one piece of data persection we can just use x.

{% highlight ruby %}
numbers_new = numbers.map {|x|}
{% endhighlight %}

The way I think about it after this point is that, we will go through each value in the array (thats our x) and for each x we are going to do what? Lets add 5.

{% highlight ruby %}
numbers_new = numbers.map {|x| x + 5}
{% endhighlight %}

Now we have an array, numbers_new, and in it we have our modified contents which if we p to the console would look like this:

{% highlight ruby %}
[10,13,28,47,66]
{% endhighlight %}