---
title: "Tripped Up With Data Types"
tags: 
- Coding practice
- Lesson learned
date: 2023-06-29T15:14:49-04:00
draft: false
---

I've taken some time this week to get back into solving coding practice problems during some downtime at school. One issue I've had with this semester is that there isn't as much coding built into the course work, so I really have to take it upon myself to find things to code. 

I was working though Project Euler [question 14](https://projecteuler.net/problem=14) where you perform iterative calculations on values up to one million. I worked out the logic, ran my code and found that the longest chain in the Collatz Sequence started at value 910107... only for it to be wrong. 

I've been tripped up before with Project Euler questions where the values are so large that they overflow the capacity of an `int` to hold them, but since I was working with values only up a million I figured it would be fine. Turns out I wasn't considering all those intermediate calculations which must have gone above 2.1 billion at some point (or 2<sup>31</sup>-1 to be more precise.) 

Long story short, I went through my code and changed most of the `int` datatypes to `BigIntegers` which didn't change the logic, but it did make everything more difficult to work with. Ran my code again and got 837799 which was... correct! 

>*Seriously, would you rather work with this:*
>```java
>if (num.remainder(new BigInteger("2")).equals(new BigInteger("0")))
>```
>
>*Or this?*
>```java
>if (num % 2 == 0)
>```

The silver lining here is that I nailed the logic of the question, but I do need to be more aware of the limitations of my datatypes since this is not the first time a Project Euler question has tripped me up like this. 

My Java code for this problem can be found on my [GitHub](https://github.com/timothynorman/projectEuler/blob/main/projectEuler/src/ca/timnorman/projectEuler/Question14.java). 