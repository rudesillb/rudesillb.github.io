---
layout: post
title:  "Arrays and Hashes"
date:   2015-9-06 10:54:34
categories: technical
---

#Overview#

According to Chapter 9 in "The Well-Grounded Rubyist" by David A. Black, arrays and hashes are collection and container objects and what he means by this is that both hold stuff! Both hold many different values that can can be selected easily in one singular place.

#Arrays#

Arrays are a list of items that are ordered. This doesn't mean that Ruby sorts them but rather Ruby knows where each value is. This means that if you have an array of grocery items:

{% highlight ruby %}
grocery = ['apples', 'bread', 'milk']
{% endhighlight %}

you can select each one of these items individually. For Example,

{% highlight ruby %}
grocery[0]
{% endhighlight %}

is going to give you apples back as a value. This is really convinient because you can always use every part of your list in a very logical way. Oh, and an array can handle numbers as well as strings too!

{% highlight ruby %}
favorite_numbers = [42 , 10^100 , 13]
{% endhighlight %}

#Hashes#

Hashes are an element that is a little harder to understand since they are common as a number list. Hashes are a list of what Ruby calles "value" and "key" pairs. Every key has a value that you can retrieve with it. This is helpful when you have a long value and you want to expedite your coding or format key inputs to values for people. First is a bit of hash syntax:

{% highlight ruby %}
state_hash = {"California" => "CA", "Maryland" => "MD"}
{% endhighlight %}