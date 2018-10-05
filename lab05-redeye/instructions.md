# Lab 5: Red Eye
*Due: Tuesday, October 9, 2018*

Your assignment is to create a program in Python (in JES) that removes "red-eye" from a picture.

## Preparations

### Find a Suitable Image

- [ ] Get a JPG image file of a person with "red-eye," preferably with relatively small dimensions - say 400 - 600px wide or so
  - Here is an example of a red-eye photo. (It's the example used in the book.)  Do **not** use this example!  Get your own.

![jenny-red](media\jenny-red.jpg)

### File Setup

- [ ] Create a new Python file named **lab05.py** and write your program in there.

## Requirements

- [ ] Create your own version of **Program 50** (page 119) in the Python book.  
  - As shown in the book, the program - one function named *removeRedEye()* - must accept six arguments

Your version of the program must also have the following:

- [ ] There must be a comment-block above the *removeRedEye()* function that briefly describes the program (one line of text will suffice)
- [ ] Throughout the program, use *variable names* that make sense to *you*.  The author uses names like `pic` for the picture object and `px` for the current pixel.  Change them!  It's okay to be more verbose.
- [ ] In the program, the `distance()` function uses the value `165`.  You should *probably* use a different value.  Adjust that number up or down to get the best results for *your* picture.  (If `165` happens to be best then that's okay.)
- [ ] Your version of the *removeRedEye()* program must use a `return` to send the altered picture object back to the test case.  
  - It's not shown that way in the book, but it's a good practice so do it.
  - Warning: be careful about the indentations!  The `return ______` statement needs to be lined-up with the FOR loop - not inside it.

### Test Case

- [ ] There must be a "test case" below the program with its own comment-block that says "TEST CASE" (Not shown in the book)
- [ ] Use the `pickAFile()` function.  Do not hardcode a filename into the test case like the professor's been doing in the in-class demos.
- [ ] Take the output from the `pickAFile()` function (assumptively a path to a JPG file) and use it as the argument for the `makePicture()` function.  
- [ ] Capture the output from the `makePicture()` function (a picture object) and store it in a variable with a sensible name of your choosing. 
- [ ] Call the *removeRedEye()* program and hard code the six arguments as shown in the book which includes the picture object, followed by the four coordinates of the red eyes in the image you're using, followed by a color.  (Hint: just use the keyword: `black` as the color.)
  - Don't make the mistake of using the book-author's X/Y coordinates.  They only work on his red-eye picture.  You must use the X/Y coordinates of the red eyes in your picture.   (Hint: use the `explore()` function to find the coordinates.)
  - Also note, be careful to choose X/Y coordinates that do not accidently wipe out the red in other places in your picture.  Only choose the coordinates of the red eyes.
- [ ] Capture the output from the *removeRedEye()* program (a new picture object) and store it in a variable with a sensible name of your choosing.
- [ ] Use the `explore()` function to display the new picture object

*Note: in the last class the professor mentioned something about using the `writePictureTo()` function to save your altered picture to your computer's hard drive as described on page 83 in the book.  Never mind that.  We'll talk about that later.*

## Get credit

To get credit for this exercise, ZIP (compress) your red-eye picture (your JPG) with your **lab05.py** file and upload the ZIP file to the **Lab 5** assignment in Blackboard.

*NOTE: the professor will take your JPG and Python file and run your program on his laptop.  If it doesn't work you'll get an immediate zero ...so make sure it works before you submit it!*

*Due: Tuesday, October 9, 2018*