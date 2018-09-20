# Lab 3: Text Manipulation
*Due: Thursday, September 20, 2018 (same day)*

Your assignment is to create a program in Python (in JES) that combines four sentences and outputs some information about them

## Requirements

### Preparations

Gather text that meets the following **requirements**.  The topic of the text can be anything you want.  You will use the text as input to the program that you will write.

- [ ] You need about 100 words in exactly four sentences.  Each sentence should be anywhere between 10 to 30 words or so.
- [ ] The first two words will be used to create a "title", so plan accordingly.  If the first two words are, "This is..." that's not going to work.  (A good example, "William Shakespeare...")
- [ ] One or more of the sentences must contain a comma.  (More is better.)
- [ ] One or more of the sentences must contain a single quote or apostrophe.  (E.g. That**'**s)
- [ ] One or more of the sentences must contain a set of double quotes.  (E.g. He said, **"**Yikes**"**)

Also, if you copy and paste from a webpage or Word Doc, look out for special characters like curly quotes, long dashes, and other non-standard characters.  Delete or replace them!

**Here's an example.**  (You cannot use this example!  Get your own.)

```
William Shakespeare (26 April 1564 (baptised) 23 April 1616) was an English poet, playwright and actor, widely regarded as both the greatest writer in the English language and the world's pre-eminent dramatist. 

He is often called England's national poet and the "Bard of Avon". 

His extant works, including collaborations, consist of approximately 39 plays, 154 sonnets, two long narrative poems, and a few other verses, some of uncertain authorship.

His plays have been translated into every major living language and are performed more often than those of any other playwright.
```

### Output Requirements

Your goal is to create a program to output something like the following in the *Command Line* area of JES, except using your content (not Shakespeare)

![screen capture](C:\Users\rober\OneDrive\Documents\UR\2018 3. Fall - DMS 102\course-documentation\lab03-text-manipulation\media\figure1.png)

- [ ] The **first line** must say: `The title of the paragraph is: __________ ____________`<br>(using your output instead of the blanks)

- [ ] The **second line** must say: `There are ____ characters and ___ words in the paragraph`
- [ ] The **third line** must say: `The paragraph has ____ commas, ____ single quotes, and ____ double quotes`
- [ ] The **last line** (after a blank line) must say, `Here is the paragraph: `...followed by the paragraph, surrounded by quotes

## File Setup

There are new techniques demonstrated in this section.  You'll need to learn and remember them and use them for the rest of the semester.  All future labs in Python will expect you to follow a similar pattern.

### Source Code Heading

- [ ] Create a new Python file named **lab03.py**

- [ ] Use the following code (copy & paste) starting on line 1<br>Notice the way comments are used at the top to define the name and purpose of the program

  ```python
  #***************************
  # Parse Four
  # - combine four sentences and output some information about them
  #***************************
  ```

Note: in future Python Labs, you'll be required to name and describe your programs yourself.

### Basic Blocking

- [ ] Directly under the comment block, define a function named `parseFour()` as shown below, and add the following "pseudo code" that gives you hints about what must be done and where to do it
    - Notice the *four parameters* in the definition of the function
    - Notice the *return* at the bottom of the function

```python
def parseFour(first, second, third, fourth):
  # concatenate the four sentences into a paragraph

  # count the characters in the paragraph
  
  # count the words in the paragraph
  
  # count the commas, single quotes, and double quotes in the paragraph

  # extract the title of the paragraph from the first two words

  # prepare and return the output
  
  return _______  

```

...note: the blank after `return` needs to be replaced using a variable name you'll create later

### Test Case

Most Python programs you write in DMS 102 from now on will require the use of a "test case" like the one below.  

- [ ] Directly below the program (from above), copy & paste the following code into JES, under the `parseFour()` function.  This is a *test case*

````python
#***************************
# Test Case
#***************************
sentence1 = ""
sentence2 = ""
sentence3 = ""
sentence4 = ""

parsedOutput = parseFour(sentence1, sentence2, sentence3, sentence4)
print parsedOutput
````

Again, notice how the block of comments is formatted.  You should do that in future labs whenever you need to write a test case.

## Write the Program

1. Fill-in your four sentences in the Test Case section.
2. Fill-in the pseudo code in the function

## Get credit

To get credit for this exercise, upload your **lab03.py** file to the Lab 3 assignment in Blackboard.
