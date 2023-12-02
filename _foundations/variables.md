---
layout: page
title: Variables
date: 2023-12-02 17:33:30 +1100
permalink: foundations/variables/
summary: Variables allow programs to remember information while they run.
---
Variables allow programs to remember information that they work with. If you're mathematically inclined, you can think of them as the letters in algebra, or if you're old enough to remember pigeonholes. 

While each programming language is different, there are some basic types of data that they can hold:

Numbers
: Numbers are the most basic type of data. Most languages support whole numbers, such as 0, 1, 4, -7, etc. and decimals, such as 1.3, -2.4, 0.0003, 3.14. Some languages, shuch as JavaScript have one number type that stores both whole numbers and decimals, whereas other programing languages treat the two as different. Whole numbers tend to be called *integers*, and decimal numbers are referred to as *floating point*.

Text
: Bits of text are called *strings*. Strings are text that are usually enclosed with singe quotes, such as `'a string in single quotes'` or double quotes, such as `"A string in double quotes"`. Different programming languages handle them differently. Most modern languages provide helpful functions to allow you to manipulate strings.

True/False
: The True/False data type is usualy referred to as *boolean*, and can represent jsut true or false. Most languages nowadays accept the words `true` or `false`, but some older languages use 1 and 0.

Objects
: Objects are more complex types, that wrap functionalty or data. Objects will be covered elsewhere. If you have done any recent programming, there's a good chance that you have used objects without realsiing.

In the world of programming, there are two schools of thought on dealing with the type of a variable:

Strict
: Some programming languages only allow one type of data in a variable - if the variable was a string, it will always be a string, and it will tell you if you are doing something wrong, such as trying to put a string into a variable that's setup to store a number. Code such as `3 + "Apple"` are usually not allowed, though some languages will try to work out what you want to do. These languages are called *strongly typed*. 

Not strict
: Languages, like JavaScript, allow you to assign any type of data to a variable, or even change the type of data in a variable. These languages tend to automatically try to convert the type of the variable to what it thinks you want. If you want to round the number 10.2, JavaScript will treat `Math.round(10.2,2);` and `Math.round("10.2", 2);` the same. If there are situations where the language can't do the conversion, it will fail while the program is running. These languages are called *weakly typed*.

There is no correct answer on which approach is correct - there is the trade-off of flexibility against removing a class of errors that can occur as the program is running, and this is the subject of one of many holy wars in program language design. 