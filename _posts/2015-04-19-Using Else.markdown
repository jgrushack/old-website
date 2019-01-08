---
published: false
layout: post
title: "Using Else:"
---

Most people are aware that if statements work with else. What many people are unaware of is that else also works with for and while. When using it with for and while it is probably wise to consider it a "nobreak" statement.



> for n in range(2, 10): <br>
...    for x in range(2, n): <br>
......         if n % x == 0: <br>
.........             print (n, 'equals', x, '*', n/x)<br>
.........          break<br>
   else:<br>
...         # loop fell through without finding a factor<br>
...         print  (n, 'is a prime number')<br>


This code will return the else statement if the loop runs 'normally'. If n returns a remainder it will break the loop and the 'else' clause will not be run.  

Although we can use Else with all types of loops, it is probably best practice to leave it to If/Else. Using else in a FOR loop can ruin the readability of the code as someone who is not versed in this use case may find it illogical. It is also easy to accidently indent the else clause which  in the above case would run an infinite loop.

also, import Antigravity