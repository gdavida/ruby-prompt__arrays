---
title: Arrays
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is an Array?

-data object that stores an ordered list of values
( http://ruby.bastardsbook.com/chapters/collections/ )

# What are some examples of information that would be Arrays as opposed to some other data type?

Arrays STORE information, and it is kept ordered. So if some piece of information doesn't need to ever be possibly stored or accessed again, maybe arrays wouldn't be the best. OR if you are storing information but just one piece, not a collection, then you would want a variable instead of an array.

# What is one way, using Ruby, to retrieve the 6th element in an Array? How about the 8th element? What happens if you try to retrieve the value of the _9999th_ element (or some element that doesn't exist in the array)?

my_array = ["red", "pink", "orange", "yellow", "green", "blue", "indigo", "violet"]
    6th item in the array 
        my_array[5]  => blue
    8th item in the array
        my_array[7]  => violet

# The previous question asks about finding, for example, the 6th element in an Array. Is it possible to find the **-6th** (Notice the negative symbol!) element in an Array? What does that even mean?

Yes, just like with selecting characters in a string, you can find a [-6] position. It means that the list item in the list/array is -1, the second from last is -2, and so on.Yes

my_array = ["red", "pink", "orange", "yellow", "green", "blue", "indigo", "violet"]
    -6 item in the array 
        my_array[-6]  => orange

# How would you perform an operation on every element inside an Array?

my_numbers = [2, 11, 83, 6, 24, 11]
my.numbers.each { prints x * 10 }

# How do you add elements to an Array?

-use .push method 
    my_array = ["red", "pink", "orange", "yellow"]
    my_array.push("green", "blue", "indigo", "violet")
    puts my_array
    ==>
    red
    pink
    orange
    yellow
    green
    blue
    indigo
    violet
    -----------------
    
-use two << (left-angled bracket) method 
    my_array = ["red", "pink", "orange", "yellow"]
    my_array << ("green", "blue", "indigo", "violet")
    puts my_array
    ==>
    red
    pink
    orange
    yellow
    green
    blue
    indigo
    violet
    
( http://ruby.bastardsbook.com/chapters/collections/ )

# Given the Array `["Laura", "Fiona", "Tori"]`, how would you replace `"Fiona"` with `"Florence"` so that you end up with `["Laura", "Florence", "Tori"]`?

ladies = ["Laura", "Fiona", "Tori"]
ladies[1] = "Florence"
puts ladies

# What do the methods `push`, `pop`, `shift`, and `unshift` do?

-push, add something to the end of array
-pop, takes last thing off array
-shift, returns first item in array and removes it from the array, shifting other items' up in array
-unshift, adds objects to the front of array, shifting other items down

# How do you determine how many elements are in an Array?
-length method
ladies = ["Laura", "Fiona", "Tori"]
puts ladies.length  ==> 3

# How would you reverse the order of elements in an Array?
-reverse method
ladies = ["Laura", "Fiona", "Tori"]
puts ladies.reverse
    ==>
    Tori
    Florence
    Laura


# How would you convert a String `"Sumeet Jain"` into an Array `["Sumeet", "Jain"]`? How about to `["S", "u", "m", "e", "e", "t", " ", "J", "a", "i", "n"]`? How would you convert the Array back into a String?

-split to turn string to array
    name = "Sumeet Jain"
    name_array = name.split
    puts name_array

-join to turn array into string
    letters_of_name = ["S", "u", "m", "e", "e", "t", " ", "J", "a", "i", "n"]
    name_array = letters_of_name.join
    puts name_array
    
    ( http://www.dotnetperls.com/convert-ruby )