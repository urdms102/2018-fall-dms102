# Lab 6: JavaScript Events
*Due: Thursday, October 25, 2018*

Your assignment is to and a "show/hide" button to an existing webpage and power it with JavaScript.

## Preparations

- Download the [Lab 6 Starter Files (ZIP)](lab06-startup-files.zip) and un-compress the **nyc** folder on your computer.  (You can just put it on your desktop for now.)
- Open the file: **index.html** in a web browser *and* a code editor (like Sublime Text)

Review the code in the HTML file.  There's a lot going on in there, but you should be able to make out the HTML tags (elements) and how they are presented in the web browser.  

In the code, scroll down to the `<table>` element (**line 35**).  That's where we need to start to operate.

## Requirements

### The Goal

- Your assignment is to change this web document so the **data table** does *not* display when the web page opens in a web browser.  In its place, there needs to be a button that says, "Show Data Table".  

- When the button is clicked by the user, the data table should appear and the button should change its label to "Hide Data Table".  

- When the button is clicked again, the data table should disappear and the label should change back to "Show Data Table".

### Instructions

- [ ] In the HTML, directly *below* the code: `<h2 id="population">Population</h2>` insert a new line and insert a button that says, "Show Data Table"
- [ ] Add an ID to the `<button>`.  The name of the ID must be descriptive.
- [ ] On the next line down, in the opening  `<table>` tag, insert an ID.  The name of the ID must be descriptive.

- [ ] Scroll down.  In between the closing DIV tag (line 75) and the closing BODY tag (line 76) insert a few lines to make some room, and create a new SCRIPT element (opening and closing tags).

The rest of the instructions are almost identical to the last demonstration from the in-class demo on Tuesday, October 23  - the one where we used a "toggle" variable and a separate button to do the toggling.

You can use that code as a starting place, making changes as needed, keeping in mind the following differences:

- [ ] The data table needs to *not* be showing when the page loads
- [ ] When the button is clicked, in addition to changing the **inner HTML** of the table element, you need to also change the **inner HTML** of the button, from "Show Data Table" to "Hide Data Table" and vice versa when it's clicked again.  

Hint: all the changing can be done in the same Event Listener and the same IF/ELSE statement as the demo, i.e. you do not have to create any new Event Listeners or IF/ELSE statements.

## Get credit

To get credit for this exercise, ZIP (compress) your **nyc** folder and upload the ZIP file to the **Lab 6** assignment in Blackboard.

*Due: Thursday, October 25, 2018*