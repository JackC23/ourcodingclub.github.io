---
layout: post
title: Introduction to Python
subtitle: Importing and exploring data with Python, writing good scientific code
date: 2019-01-26 00:00:00
author: Declan
meta: "PythonBasics"
tags: intro_to_python
---
<div class="block">
          <center><img src="{{ site.baseurl }}/img/tutheaderintro.jpg" alt="Img"></center>
        </div>

### Tutorial aims:

#### 0. Understand why Python is so useful for scientific programming

#### 1. Learn how to import tabular data

#### 2. Learn how to apply the same operations to multiple values

#### 3. Learn how to store many values together

#### 4. Learn how to perform the same operations of many different values

#### 5. Making programs do different things based on different values

#### 6. Learn about functions in Python

#### 7. Learn how to deal with errors in Python

#### 8. Making programs more reliable

#### 9. Learn how to debug scientific code

#### 10. Learn how to write Python programs for the command line


## Why Python for scientific programming?

You may have heard about the Python programming language before. It is often talked about as the next "Up and coming" programming language, or described as being a new, "trendy" programming language that everyone should be learning, particularly scientists. I am going to argue that Python is no longer merely "up and coming", or even particularly new, but one of the most popular and useful programming languages you could invest time in learning. In fact, as of 2018, Python is (by certain measures) **the most widely used programming language in the world**. So if you are a scientist, researcher, or student doing any kind of data analysis, or numeric programming, then I think Python is worth investing some time in learning, even just the basics.

Python is a programming language, a tool used to make computers do useful things for scientific coders much faster than they could do using conventional tools like spreadsheets or plotting software (and certainly much faster than manual calculations!). But programming languages are not really designed for computers at all. In fact, your computer has no idea what all the words and symbols in a piece of code written in Python actually *mean*. (It only understands ones and zeros and electrical currents.) [footnote]. The reason is that programming languages are actually designed for *humans* to have a convenent way of programming a computer without getting involved in things like binary and hexadecimal codes, and worrying about electronic circuitry inside the computer. 

## Why Python?

### 1. Readability

Python shines because it is designed to be *readable* for us humans. Python is often described as a language that is intuitive and relatively easy to learn. The **syntax** (how you arrange the set of words and symbols to make a Python program) is meant to be intuitve to humans by being similar to natural human languages in many ways. For example, look at these little snippets of Python and see if you can guess what they mean and what might happen if we told the computer to run the code:

```
"Python".startswith("P")
```
This bit of python code reads like: *Python starts with a "P"*, and that is exactly what it means  in Python!. If we ran this bit of code, the computer would print out `True` on the screen.

What about this one?

```
"thon" in "Python"
```
(Imagine reading it like a question...)

So if we ask: *"thon" in "Python"?*, the answer is yes (or True), because the letters "thon" appear in the word "Python". If we wrote:

```
"xyz" in "Python"
```
we would get False, because those letters are not in the word "Python".

Python syntax has many more similarities with natural languages, and we will discover more throughout this tutorial. Hopefully this will make learning the Python language more intuitive (and fun, as we can compare it to human languages (well, English...)).

Here is one more bonus round. Can you guess what might happen if we ran this Python code?

```
tastyword = "chocolate"
x = 3

if tastyword.count("o") < x and tastyword.endswith("e"):
  print("You have won some tasty chocolate!")
```
>
### 2. General Puropose

Python has a major advantage when compared to some other commonly used programming languages in the scientific community; it is a *general purpose* programming language. Compared to other languages such as Matlab, IDL, ncl, and R, which were designed with specific applications in mind, Python was built as a general purpose programming language (like Java, C, Ruby etc.). This means you can use Python to write your data analysis code, plot the results of the analysis, write a numerical model, run a website, do your tax return...the list goes on. 

Because of it's general-purpose design, Python is used in the real world in a range of industries. Python is used by scientists at universities across the world, developers at big tech companies like Amazon, Facebook, and Google, by financial services companies, and social media apps like Facebook and Instagram, for example. In short, while this tutorial focuses on scientific applications of Python, you are learning a programming language that has a huge variety both within and outwith the scientific community.

### 3. Scientific Python Community

The third reason I'm going to mention is the community behind Python. As mentioned before, writing code is as much a way of communicating between humans trying to solve the same scientific problems as it is telling the computer what to do. Python has a very friendly and active community supporting it, many of whom are found on internet resources such as forums and the popular StackOverflow Q&A site. 

If you are stuck with a problem in Python, online resources are so plentiful that is often enough to just type "How do I do _X_ in Python", into a search engine - the first few results often will contain your answer. (And often the top link is a StackOverflow question asked by someone with the same or very similar problem to you.

In the domain of science, the Scientific Python community is just as well established. You may have already heard of Python packages like Numpy (Numerical Python), SciPy (Scientific Python), as well as other tools like Pandas, matplotlib, and others. Many of these tools were developed by scientists to share something back to the Python community, and they have now grown and become almost _de facto_ standard tools within the scientific programming community. 


