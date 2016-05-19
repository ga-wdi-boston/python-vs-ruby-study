# Ruby vs Python Study

In this study we are going to to ino the differences between Ruby and Python.

## Required Readings

Please Perform readings after reading this this page.  Follow along using a
Python repl

-   [Code School: Try Python](https://www.codeschool.com/learn/python)
-   [Learn Python the Hard Way](http://learnpythonthehardway.org/book/)
    Exercises: 13, 18, 21, 30, 32, 34, 39, 42, 44
    All exercises are quite short

## Variable Declaration

Similar to Ruby, in Python we ***DO NOT*** have to declare our variables with
something like a `let` or `const`. Consider the following:

```ruby
# Ruby
kitty = "Mr.Kitty"
i_am_ten = 10

puts kitty
# => "Mr.Kitty"
```

Python is almost identical to Ruby in this manner.

```py
kitty = "Mr.Kitty"
i_am_ten = 10

print kitty
# => "Mr.Kitty"
```

I can also do something cool when I declare my variables: simultaneous
declaration.

```py
a,b = 3,4

# a = 3
# b = 4
```

## Lists (Kinda like arrays)

It's important to note a list is not an array.  It looks like an array, acts
like an array but an array in Python is a module that concerns itself with
efficiency.

We'll stick with lists, they are similar to the array type we have used in
both Javascript and Ruby.

Take a look at how we make a list and append things in Python, it should look
familiar to how we did things in Ruby:

```py
 cat_list = []
 cat_list.append("Mr.Kitty")
 cat_list.append("Dr.Fuzz")
 print cat_list

 # => ["Mr.Kitty", "Dr.Fuzz"]
```

Lets take a look at looping through that list:

```py
cat_list = ["Mr.Kitty", "Dr.Fuzz", "Admiral Meow", "Meowbama"]

for cat in cat_list:
    print cat

print "That's a lot of cats"

# => Mr.Kitty
# => Dr.Fuzz
# => Admiral Meow
# => Meowbama
# => That's alot of cats
```

## Dictionaries

Dictionaries in Python are pretty similar to hashes in Ruby.  I say pretty
similar because there are minor behavioral difference between the two, but for
now we'll think of dictionaries and hashes as one in the same.

First here is a Ruby hash:

```ruby
cat_hash = {'Jason' => 'Mr.Kitty', 'Lauren' => 'Admiral Meow', 'Antony' => 'Meowbama'}

cat_hash['Jason']

# => "Mr.Kitty"
```

And now be prepared to have your mind blown by a Python dictionary:

```py
cat_dict = {'Jason' : 'Mr.Kitty', 'Lauren' : 'Admiral Meow', 'Antony' : 'Meowbama'}

cat_dict['Jason']

# => "Mr.Kitty"
```

When you play around with hashes you may notice that the return dictionary may
be in a different order then when you entered it.  This is one of those
differences between Python dictionaries and Ruby hashes, order isn't guaranteed,
but hey, its a dictionary if you're using it for order there is a better way.

Adding key/value pairs to a dictionary is exactly the same in both Ruby and
Python.

```py
cat_dict = {'Jason' : 'Mr.Kitty', 'Lauren' : 'Admiral Meow', 'Antony' : 'Meowbama'}

cat_dict['Ross'] = "Dr.Fuzz"

cat_dict
# => cat_dict = {'Jason' : 'Mr.Kitty', 'Ross': 'Dr.Fuzz', 'Lauren' : 'Admiral Meow', 'Antony' : 'Meowbama'}
```

And let's delete Ross... Because Ross

```py
cat_dict = {'Jason' : 'Mr.Kitty', 'Ross': 'Dr.Fuzz', 'Lauren' : 'Admiral Meow', 'Antony' : 'Meowbama'}

cat_dict.pop('Ross')
# => 'Dr.Fuzz'
```

Now that Ross is gone let's print all of the values in our dictionary:

```py
pet_hash = {'Lauren': 'Admiral Meow', 'Antony': 'Meowbama', 'Jason': 'Mr.Kitty'}

for key in pet_hash:
	print(pet_hash[key])

# The word "key" is arbitrary here, it could be "bob" or "foo" and it would
# behave the same.

# => Admiral Meow
# => Mr.Kitty
# => Meowbama
```

## Basic Syntax

You may have noticed from a few of the examples that Python is very similar to
Ruby, however a key difference is syntax *** WHITE SPACE MATTERS***

In Ruby we closed blocks with the `end` keyword:

```ruby
def foo
  #some code
end
```

In Python as we open blocks we have to indent:

```py
def foo(x):
  print x
  if x > 0:
    return x
  elif x == 1:
    return x-1
  else:
    return x+1

def bar:
  print "Hello"
```

Please note:

-   The use of a semicolon when declaring functions
-   The clean indentation (Python will throw in error if you do not use correct
    indentation)
-   Properly declaring same level functions

In Ruby poor indentation is a sign of poor code quality, however in Python poor
indentation will throw an error.  ***BE VIGILANT WITH YOUR INDENTATION***

## Strings

In Ruby for string interpolation we did something like

```ruby
cat = "Mr.Kitty"

puts "#{cat} is actually quite dumb"
# => "Mr.Kitty is actually quite dumb"
```

For Python there are two ways to do this, in Python 3.5 this is the prefered way

```py
title = "Mr"
name = "Kitty"
string ="{}.{}".format(title,name)
print(string)
# => "Mr.Kitty"
```

In earlier versions of Python this was the prefered way, but it is still used
frequently

```py
title = "Mr"
name = "Kitty"
"%s.%s"%(title,name)
# => "Mr.Kitty"
```

Here are some commonly used argument specifiers

```bash
%s - String (or any object with a string representation, like numbers)
%d - Integers
%f - Floating point numbers
```

## Installing packages

Remember in Ruby how we used `gem install <Gemname>` well Python has something
similar called `Pip`.

In ruby we would run:

```bash
gem install cative_record
```

In Python we go about this by using

```bash
pip install cative_record
```

Booom you just installed a package!
