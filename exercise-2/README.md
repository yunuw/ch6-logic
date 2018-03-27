# Exercise 2

In this exercise, you'll practice writing conditional statements in Python. In particular, you should complete the following questions on [Codingbat](http://codingbat.com/python), which a website (one of many) for practicing basic programming.

1. [no_teen_sum](http://codingbat.com/prob/p100347)

	```python
	#solution
	def no_teen_sum(a, b, c):
		return fix_teen(a) + fix_teen(b) + fix_teen(c)

	def fix_teen(n):
		if 13 <= n <= 19 and n != 15 and n != 16:
			return 0
		else:
			return n
	```

2. [lucky_sum](http://codingbat.com/prob/p107863)

	```python
	#solution
	def lucky_sum(a, b, c):
		if a == 13:
			return 0
		elif b == 13:
			return a
		elif c == 13:
			return a+b
		else:
			return a+b+c
	```

3. [make_brick](http://codingbat.com/prob/p118406). Note that you may not need to use conditional statements for this, but it's good practice at the kind of logical, abstract thinking used in programming!

	```python
	#solution
	def make_bricks(small, big, goal):
  		num_big = min(goal//5,big)
  		num_small = goal - num_big*5
  		return num_small <= small
  	```

Feel free to practice with the other problems as well!
