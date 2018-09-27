# Lab 3: Text Manipulation
*Due: Thursday, September 27, 2018 (same day)*

Your assignment is to create a program in Python (in JES) that reduces the amount of red in a picture

## Requirements

### Preparations

- You'll need an JPG image file, preferably with relatively small dimensions - say 400 - 600px wide or so

### Output Requirements

Your goal is to create a program that accepts a *picture object* as an argument and **return**s a *picture object* that's had the red in each pixel reduced by 50%

## File Setup

- [ ] Create a new Python file named **lab04.py**

### Source Code Heading

- [ ] Use the following code (copy & paste) starting on line 1

  ```python
  #***************************
  # Decrease Red
  # - reduce the amount of red in a picture
  #***************************
  ```


### Basic Blocking

- [ ] Directly under the comment block, define a function named `decreaseRed()` 
- [ ] Set the function so it accepts one parameter named `pictureObject`
- [ ] The last line of the function will **return** the `pictureObject`

### Test Case

- [ ] Directly below the program (from above), copy & paste the following test case

````python
# *************************************
# TEST CASE
# *************************************
file = pickAFile()
picture = makePicture(file)
lessRedPic = decreaseRed(picture)
explore(lessRedPic)
````

## Write the Program

Here is some pseudo code.  For more help, see Program 34 in the book (page 89)
````python
def decreaseRed(pictureObject): 
  # get all the pixels from the picture put in a list - use getPixels()

  # loop through each pixel in the list one-by-one - use a FOR loop

  	#in the FOR loop, get the red value of the current pixel - use getRed()

    #reduce the red value by half - use setRed() and a multiply by factor of 0.5
    
  #return the altered picture
  return pictureObject
````

## Get credit

To get credit for this exercise, upload your **lab04.py** file to the Lab 4 assignment in Blackboard.
