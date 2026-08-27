# ECE 2112 - EXPERIMENT 1: Introduction to Python Programming

HUIT, THIMOTY JOSHUA O.

2ECE-B

8/27/2026

## Objective of this Activity

The objective of this experiment is to develop basic python programming skills by applying fundamental functions, operators, and string operations. This activity also aim to develop the ability to manipulate strings by using indexing, slicing, and built-in string methods, and also construct simply python functions.

This experiment is divided into three problems which are: **Word Rotation, Username Builder, Bookend Swap**

## A. Word Rotation Problem

### This Code: 

	def rotate_word(text):

  		return text[1: ] + text[0]

This code explains that this **rotate_word()** function takes a string and moves its first character to the end of the word. 

for **text[1: ]** it uses string slicing to get all the characters starting from index 1 until the end of the string.

for **text[0]** it uses the string indexing to get the first character.

for the operations the **+** operator combines the sliced string and the first character, and the **return** statement returns the newly arranged word.

Example:

	def rotate_word(text):
	
		return text[1: ] + text[0]

	print(rotate_word("Ipad"))

If you execute this it will show you: **"padI"** 

Therefore, the main purpose of this def rotate_word() is to rotate a word by getting the first character and putting it into the end of the word.

## B. Username Builder Problem

### This Code:

	def make_username(first_name, last_name):
		first_name = first_name.lower().replace (" ", "")
		last_name = last_name.lower().replace (" ", "")

		return first_name + "." + last_name

This code explains that the make_username function takes a first name and last name and converts them into a username.

For both first_name and last_name the reason we use .lower() is to converts all of the characters that are in uppercase into lowercase letters, and for the .replace(" ", "") this removes the spaces by replacing every space " " with an empty string "".

After it processed those two names the function now use the

	first_name + "." + last_name

to combine them and turn them into a username. The "." is included to place period between the first and last names.

Example:

	make_username("Thim", "Huit")
This name will be processed into thimhuit and now it is processed the function will use the 

	first_name + "." + last_name

which will result to thim.huit

Therefore, the main purpose of this def make_username(first_name, last_name) is to turn a name into a username lowercase letters 

## C. Bookend Swap Problem

### This Code:

	def swap_bookends(items):
		first, *middle, last = items

		return [last] + middle + [first]

This code explains that the swap_bookends() function takes a list and exchanges the positions of its first and last elements while keeping the middle elements in their original order.

So for visualization think of it like this

You have: 

	[1, 2, 3, 4, 5, 6] 

and by using this code swap_bookends()

it will swap the first and last number but retaining the middle part like this:

	first = 1
	middle = 2,3,4,5
	last = 6

So the result will be:

	[6, 2, 3, 4, 5, 1]

Therefore, the main purpose of this def swap_bookends(items) is to exchange the first and last elements but keeping the middle elements in their original order.

## Conclusion

This experiment shows that the use of basic python operations for manipulating such as strings and lists. These three problems apply string indexing and slicing, built-in string methods, string concatenation, and extended sequence unpacking to produce the required results.
