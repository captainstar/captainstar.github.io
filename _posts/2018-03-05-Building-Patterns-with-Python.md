---
title: Building Patterns with Python
layout: post
author: anshu.attavar
permalink: /building-patterns-with-python/
source-id: 1daA42mwY6nW6Z9OoPzgKw2dqLQORzHD21-NYYJ5R2eQ
published: true
---
This lesson we started to learn how to program with python but in a more complex way than last year. 

 Firstly we went on to a website called repl.it which lets you code and test what is going to happen and spot any errors with your code and lets you run it. In the lesson we programmed a turtle to draw shapes.

We imported it, then set its speed:

import turtle

turtle.shape("turtle")

turtle.speed(100000)

Then we made it able to draw any sided shape with this code which all you had to do was state the side number and length.

def draw_shape(sides,length):

  for number in range(sides):

    turtle.forward(length)

    turtle.left(360/sides)

Then I made it draw a cool endless pattern:

side = 1

while True:

  draw_shape(7,side)

  side = side + 0.7

  turtle.left(10)

![image alt text]({{ site.url }}/public/tpI8LUeAjEQuHtgeP6ag_img_0.png)

