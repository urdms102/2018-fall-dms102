# DMS 102 Homework: Chapter 8

Assignment: read and try the programs in **Chapter 8, Modifying Samples in a Range**

- Yes, the entire chapter!  But it's not so bad.  It's 19 pages and its really just application of the same things we did earlier but in a different context (samples instead of pixels).
- Suggestion: dive right into the programs.  Read/skim just enough of the text around the programs to understand what they're demonstrating, and try them out in JES.  
- Get all of Chapter 8 done before you go on break next week.*  When we get back, the in-class assignments we do will assume you've tried all those programs.  If not, you'll be lost.  (And you'll lose points.)

\* Of course you can do all this while you're on break, but who wants to do that?  Seriously, get this done *before* you go on break.  We'll hit the ground running right when we get back together on November 27.

Although there are 11 programs, they're all just variations of the a few topics. (See below).  Also see my hints & tips at the very bottom of this post.

## Looping through all the samples using index

- Program 99: Increase an Input Sound’s Volume Using range
- Program 100: Increase the Volume, Then Decrease It
- Program 101: Increase the Volume, Then Decrease, Using Index Notation

## Merging sounds (words) together

- Program 102: Merging Words into a Single Sentence
- Program 103: Merging Words Using Index Notation
- Program 104: Splice the Preamble to Have United People

## Clipping and copying sounds

- Program 105: Create a Sound Clip
- Program 106: General Copy
- Program 107: Using the General Clip and Copy

## Changing the order of samples

- Program 108: Play the Given Sound Backwards (Reverse It)
- Program 109: Mirror a Sound Front to Back

# Kostin's Hints & Tips

When trying the programs as written in the book, keep in mind that the author is somewhat inconsistent in the way he presents the sample programs. 

In addition to what the author suggests, also do the following:

- Find these files in your **mediasources**  folder and copy them to your computer's Desktop
  - **preamble10.wav**
  - **guzdial.wav**
  - **is.wav**
- When you first open JES, in the command line, type: `getMediaPath()` It should display a path to your computer's desktop.  
  - **If not**, then you need to fix it.  Copy the path that was displayed at the command line and enter this on the next line (and don't press ENTER yet): `setMediaPath()` (notice, that's **s**etMediaPath with an "s", not **g**et) 
  - And then between the parenthesis, paste AND EDIT the path to point it to your computer's desktop, something like this:<br>`setMediaPath('C:\\Users\\PATHTODESKTOP\\Desktop')` ...for Windows<br>`setMediaPath('\\Users\\PATHTODESKTOP\\Desktop')` ...for Mac<br>
- As you try the programs in Chapter 8, work right on your computer's desktop (in the same place as the .**wav** files) and create new **.py** files; e.g. **program99.py**

## Programs 99-101

For Program 99, 100, and 101, use a set of #TEST code like this:

```python
#TEST
file = getMediaPath("preamble10.wav")
sound = makeSound(file)
increaseVolumeByRange(sound)
explore(sound)
```

Edit the TEST code above as needed for Programs 99 - 101 *(Note: you'll need to change the program name - second line from bottom - for each one)*

## Programs 102 -104

For Programs 102, 103, and 104, whenever the author writes `makeSound("preamble10.wav")` within a program you need to replace it with this:`makeSound(getMediaPath("preamble10.wav"))` (or `"is.wav"` as needed)

For Programs 102, 103, and 104, use #TEST code like this:

```python
explore(merge())
```

...or merge2 ...or splicePreamble() as needed.

Also, beware when typing Program 103.  In the book, it spans two pages.  Just keep in mind that the line under the FOR loop is supposed to be indented!

And when typing Program 104 which is also split across two pages, the lines `target=` ...and `targetIndex=`...are supposed to line-up, one directly under the other (no indent)

## Programs 105-107

For Programs 105, 106, and 107, put ALL THREE in one file (e.g. name it **program105-106-107.py** or something like that.)

In the one file, write each program one under the other, and then at the bottom, use #TEST code like this:<br>`explore(createNewPreamble())`

Notice how the third program *uses* the previous two.  That's because the first two programs are written using a concept called *abstraction*.  (Hint: that's a concept you'll see on the final exam!)

NOTE: in this area of Chapter 8 (under Program 107), there's a section you should read but you can skip trying out.  Using `media import` is not something we need to do in DMS 102.  

## Programs 108 and 109

The last two programs does some more interesting techniques to alter the arrangement of the samples, more of which you'll see in Chapter 9 and beyond.  

For Program 108, you can use a #TEST case like this:

```python
# TEST
file = getMediaPath("preamble10.wav")
sound = makeSound(file)
explore(reverse(sound))
```

And for Program 109, you can use a #TEST case like this:

```python
# TEST
file = getMediaPath("preamble10.wav")
sound = makeSound(file)
mirrorSound(sound)
explore(sound)
```

# General Advice

As always, if you're trying some program and it's just not working for you, STOP - don't hack away for more than say, 20 minutes on one thing.  Go to **Slack** and upload your code (you upload files in Slack), into the **#help** channel and describe the problem you're seeing.  Someone (or I) will get back to you shortly.