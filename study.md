# Ruby vs Python Study

In this study we are going to to ino the differences between Ruby and Python.

## Required Readings

-   [Example Reading](https://www.github.com/ga-wdi-boston/example)
-   [Example Reading](https://www.github.com/ga-wdi-boston/example)
-   [Example Reading](https://www.github.com/ga-wdi-boston/example)

## Variable Declaration

Similar to Ruby and different then Javascript, in Python we do not have to
declare our variables with something like a `let` or `const`. Consider the
following:

```js
// Javascript
var kitty = "Mr.Kitty";
var iAmTen = 10;

console.log(kitty);
// => "Mr.Kitty"
```

```ruby
# Ruby
kitty = "Mr.Kitty"
iAmTen = 10

puts kitty
# => "Mr.Kitty"
```

Python is almost identical to Ruby in this manner.

```py
kitty = "Mr.Kitty"
iAmTen = 10

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
like an array but an array in Pyton is a module that concerns itself with
effiency.

We'll stick with lists, they are similar to the array type we have used in
both Javascript and Ruby.

Take a look at how we make a list and append things in Python, it should look
familar to how we did things in Ruby:

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

print "That's alot of cats"

# => Mr.Kitty
# => Dr.Fuzz
# => Admiral Meow
# => Meowbama
# => That's alot of cats
```

## Basic Syntax

You may have noticed from a few of the examples that 

```md
<!-- your answer here -->
```
