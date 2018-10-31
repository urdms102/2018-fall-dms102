# Lab 8: JavaScript Plugins
*Due: Tuesday, November 6, 2018 (one week)*

Your assignment is to edit the starter files, provided, to install two plugins.

## Preparations

Typically, you need to research your own libraries and plugins, decide what you want to use, then learn how to use them, and download the source code.  For this lab assignment, you're being provided with all the files and information for these two plugins:

- **jQuery UI, Accordion** (from: [jqueryui.com/accordion](https://jqueryui.com/accordion/))
- **Fotorama** (from: [fotorama.io](http://fotorama.io/))

You don't have to do anything with those websites.  Just follow the instructions below.

- [ ] [**Download the file: nyc3.zip**](nyc3.zip) and unzip the folder **nyc3** (put it wherever you want to do your work)
- [ ] Also [**download the file: plugins.zip**](plugins.zip) and unzip the folder **plugins** to a *different* area
  - Do *not* put the **plugins** folder inside the **nyc3** folder.  Leave it separate.
- [ ] In the **nyc3** folder, create a new sub-folder named **js**
- [ ] From the **plugins** folder, get the _three_ .js files (**fotorama.js**, **jquery.js**, and **jquery-ui.js**) and move them into the **js** folder
- [ ] From the **plugins** folder, get the _two_ .css files (**fotorama.css**, and **jquery-ui.css**) and move them into the **css** folder
- [ ] From the **plugins** folder, get the remaining **images** folder (and its contents) and move it into the **css** folder too
  - You can delete the **plugins** folder when it's empty
- [ ] Open the **index.html** file in a web browser
- [ ] Also open the **index.html** file in your code editor (possibly *Sublime Text* if that's what you're using)

## Requirements

### The Goal

- The goal is to transform the existing, static webpage (below, left) into a dynamic webpage, powered by two jQuery plugins: "Fotorama" and "jQuery UI, Accordion" (below, right)

![Screen capture](media\nyc.jpg)

*As shown in Tuesday's lecture, the plugins will power a slide show for the images, and the "accordion" function on the three sections: Introduction, About, and History*

## Step 1: Install the Library (jQuery)

Usually, you would have to go to the library's website and download the source code and put it into your file system.  You don't have to do that because the files have already been provided and you installed already in the Preparations section, above.  So continue by installing the files into the HTML...

- [ ] In the **index.html** file, install the jQuery library in the appropriate place using the `<script>` tag
  - Remember to use the path `src="js/jquery.js"` (with the "**js/**" part) because the file is in a sub-directory

## Step 2: Install the Two Plugins (jQuery UI and Fotorama)

- [ ] In the **index.html** file, install the plugins: **jquery-ui.js** and **fotorama.js** in the appropriate place using the `<script>` tag
  - Note: although *order matters* between the library and the plugins, order does *not* matter among the two plugins, i.e. it doesn't matter which plugin goes above the other - jQuery UI or Fotorama
  - Also remember the "**js/**" part of the path for the plugin files because they're in a subdirectory named **js**

## Step 3: Install the Styles (CSS files) for the Two Plugins

In this case, both plugins are require the use of CSS files (which you've already installed in the file system).  So continue by installing the CSS files in the HTML...

Here is the line of code you need for jQuery UI's styles:

`<link rel="stylesheet" href="css/jquery-ui.css">`

And here is the line of code you need for Fotorama's styles:

`<link rel="stylesheet" href="css/fotorama.css">`

- [ ] Install both lines of code in the appropriate place in the HTML - directly between the TITLE tag and the existing LINK tag.
  - Just create a couple lines under *Line 7* and put the LINK tags there

## Step 4: Initialize the Two Plugins

First, initialize the jQuery UI's Accordion.  Here is the line of code you need:

`$("#accordion").accordion();`

- [ ] Put that line of code in the appropriate place in the HTML between another set of `<script>` tags
  - Note: for the purposes of this lab assignment, you won't need any options for the accordion



Next, initialize the Fotorama plugin.  Here are the lines of code which include an option array:

```javascript
$('#slideshow').fotorama({
	autoplay: true,
	arrows: false,
	nav: false,
	transition: "dissolve"
});
```

- [ ] Put those lines of code in the appropriate place in the HTML between another set of `<script>` tags

## Step 5: Arrange the Content as Prescribed by the Two Plugins

### Setup the Accordion

In the webpage, the three sections, "Introduction", "About", and "History" are already setup in the prescribed pattern: one wrapper (a SECTION tag) with repeating pairs of two elements: an H2 followed by a P tag.  That'll work nicely with the accordion function.  You just have to do one more thing to get the accordion to work...

- [ ] The initialization string for the jQuery UI, Accordion function (in Step 4) assumes the element you want to turn into an accordion has an ID of "accordion".  So add the `id="accordion"` attribute to the appropriate element in the HTML

### Setup the Fotorama Slideshow

In the HTML, you'll see one IMG tag up near the top of the code, directly under the line: `<h1>New York City</h1>`.  There are four more image files in the images folder.  You need to add them to the HTML.  Here is the code:

```html
<img src="images/brooklyn.jpg" data-caption="Brooklyn">
<img src="images/bronx.jpg" data-caption="Bronx">
<img src="images/queens.jpg" data-caption="Queens">
<img src="images/staten-island.jpg" data-caption="Staten Island">
```

...add these lines of code directly under the existing IMG tag.  (Just move the `</header>` down a few lines.)

According to the Fotorama website, you need to wrap all the images you want in the slide show inside one HTML element (a `<div>` will do) and give that element an ID of "slideshow"

- [ ] So add a couple of lines above and below the list of images, insert the opening and closing DIV tags, and add the `id="slideshow"` attribute in the appropriate spot.



If you've installed everything correctly, when you open the webpage in a browser, you should see the five-slide slide show in the top-right area, and the three sections on the right should work as "accordions."

## Get credit

To get credit for this exercise, ZIP (compress) your **nyc3** folder and upload the ZIP file to the **Lab 8** assignment in Blackboard.

*Due: Tuesday, November 6, 2018 (one week)*

