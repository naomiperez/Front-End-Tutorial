# How to Create A Basic Project Portfolio with an HTML Website on CodePen

## Introduction
In this tutorial, you will be creating your first webpage. We will be using the web programming languages HTML and CSS to create a personal webpage with descriptions of your own computer science projects. The webpage will be responsive, meaning the text (and spaces between the text) will grow and shrink proportionally to the size you stretch the browser page to be. We’ll see how this works later in the tutorial. This will make the website more visually appealing! Having a personal portfolio of projects is very important when you are applying to colleges or jobs in the future, so that you can demonstrate to admissions officers or employers what you can do with the skills you learned in this course.

### Materials You Will Need
A computer with a browser installed like Chrome or Safari

Notes: 
The example code in the technical overview and for each step in the instructions will be shown in a different font with a yellow background. 
In the Instructions section, the text highlighted in a slightly darker grey tone is the new code that we have added in each step.

## Technical Overview
In this tutorial, we will only be creating a static website, meaning the page will always look the same whenever you view it, unless you change your code later. We won’t be covering the alternative to static programming, which is dynamic programming (https://www.geeksforgeeks.org/difference-between-static-and-dynamic-web-pages/).

### Overview of HTML
We will be using HTML, which stands for Hypertext Markup Language, to allow the document we design to be displayed in a webpage. HTML creates the basic elements of a static website, like the structure of the website, where the elements are placed in the page, and the text, links, images, etc. 

### HTML Elements
HTML code is made up of elements, which define the structure and content of the webpage, such as paragraphs, headers, titles, etc.

### HTML Tags
HTML code uses tags to represent elements. A tag is a keyword surrounded by a less than sign < and a greater than sign >. These tags are recognized by the computer and converted into webpages you see on the internet. An example of a tag is the <body> tag, which designates an area of the webpage to display the main content of the web page. Most HTML tags need both an opening tag and a closing tag to store content inside. The opening tag is exactly what I described with the greater and less than sign, and the closing tag is just the same syntax as the opening tag, except with a backslash after the less than sign. For example:
	opening tag →   ```HTML <body>  </body>```   ← closing tag

Webpages are written by creating many of these elements, and nesting information and other elements within them. Nesting HTML elements just means that you are placing (or typing) elements within the opening and closing tag of other HTML elements. For example, we can create a <body> element and nest a paragraph element within it using the <p> tag like so:
<body>
<p> Text here will be displayed in a paragraph format. </p>
</body>
Note: The indent on the <p> tag is not necessary for the code to work, but it helps a lot to read the code when there are many tags nested within one another.

You can read more about HTML tags at https://www.w3schools.com/tags/default.asp

### CSS: Styling the Webpage
The other language we will be using is CSS, or Cascading Style Sheets, which allows us to add more formatting and design elements to the page, like spacing between elements of the webpage, colors, fonts, etc. In CSS, we use selectors to select elements of the HTML and add style rules to them. We select HTML elements to style them using the tag keyword followed by opening and closing curly braces { }. For example, if we want to style the text within the paragraph <p> tag, we type this into our CSS section of code:
			```CSS p {
			   
}

If we wanted to add a style property for this paragraph element, we must write it within these curly braces. There is a list of properties you can choose from to define for each HTML element. For example, for our paragraph, we could define the properties “color”, “font-size”, and “margin”. To assign a value to a property, we type a semicolon after the property name, like so:
			```CSS p {
			    color: red;
}```

You can read more about CSS selectors at: https://www.w3schools.com/css/css_selectors.asp

### CodePen
	In this tutorial we will use a website called CodePen (codepen.io) to create our website. CodePen is an online text editor in which we can write HTML and CSS and the resulting web page will display right next to our code.

## Instructions
Open a browser and type in codepen.io
If you already have an account, click “Pen”


If you don’t have an account yet, you can start coding right away by clicking on the “Start Coding” button



Now you should see the text editor with 3 sections: HTML, CSS, and Javascript. Your screen should look like this (the red text is annotations, you shouldn’t see those on the screen):

 

Note: On your screen, the sections on the left will probably be white, not yellow.

In the HTML section, add an opening and closing <html> tag by typing:


This element defines our code as html code. We will nest all other elements inside this tag.

Next, nest a <head> tag within the <html> tag. This will contain some metadata about our HTML document/code. Metadata is not content that will be visible on the webpage, but will provide the browser information about your webpage content. For example, we can add a <title> tag within the <head> tag to tell the browser that we’ve given a name to our webpage, like so:



You can change the “Your Name Portfolio” to your actual name.

Note: Remember that the indentations we’ve added (as well as the words being all lowercase) aren’t necessary for our code to work. They just make the code easier to read. 

We also need to add a tag called <meta> in order to make our page responsive. You can see that this tag has some extra text next to the name. These are attributes of the tag, which add more information about the tag. We won’t be using attributes in the rest of the tutorial, so it’s okay if you don’t fully understand this tag.



The width=device-width attribute “sets the width of the page to follow the screen-width of the device” 
The “initial-scale=1.0” sets the initial zoom level when the page is first loaded by the browser. 
You can read more about HTML attributes here: https://www.w3schools.com/html/html_attributes.asp

Now, type in a <body> tag. This is where the bulk of our webpage’s content will go. This element usually comes after the <head> tag in HTML code.


Since we’re making a personal portfolio, we will probably want to display our name at the top of the webpage, with some heading like “Naomi’s Portfolio”. To do this, add an <h1> tag. This will make the text within the tag large, like a header.


This is the first bit of content that will be visible on the page! Note that the content in our <body> tag is not styled with CSS yet, so it may look a little ugly. It should look like this: 



Now, we’ll add our first project title and description. To do this, add an <h2> tag. The <h2> tag is a header element like <h1>, except the text nested within the tag will look slighty smaller on the web page. We will also add our project description in plain text, and since that text is within the <body> tag, it will be displayed on our webpage, too.


So far, your web page should look like this:



To add more projects, just add a new <h2> tag after your last project description, and new project description after that. For example:



Now, we will style our page with CSS! CodePen automatically links the CSS to the HTML, so all we have to do is type our CSS style properties into the CSS section of the CodePen text editor.

To add style to the body tag, type this block of code into the CSS section (labelled “CSS”, located below the HTML section).

 

Here, we used the CSS selector feature of the language to select the body element from our HTML and add some rules to style the text and elements in it. The properties in this block of code are “text-align” and “font”. For “text-align”, we define that we want the text to be aligned in the center by typing “center” after the colon. For “font”, we define the size of the font, then type a space, then type the font family name. It’s important to end each styling rule with a semicolon. 
	Since all of the text we added is nested within the body tag, these properties will apply to everything we have displayed on our web page.

Now, your web page should look like this:



All of the text in the body of the page is centered, and in Georgia font. This is our final product! 

You can click the “Save” button at the top of the screen to save your project to your CodePen portfolio.



## How Our Web Page is Responsive
Notice the “vw” next to the “2.5” font size in our CSS. 

This is the unit of the font size. We could type out “px” which stands for pixels. When we use “vw” instead of “px”, we are telling the browser that we want the font size to be proportional to the size of the browser window. If we had used “px”, the font would always be a fixed size. 

1vw = 1% of the window width
2.5vw = 2.5% of the window width
10vw = 10% of the window width
etc…

You can test this by shrinking or expanding the window size, and you will notice that the text shrinks and expands with it, rather than staying the same size. You can see in this screenshot that I’ve shrunk my window and the size of the text shrunk too:



## Conclusion
	You’ve now created your first responsive personal webpage to demonstrate your computer science projects. Congratulations! In this tutorial, we covered a lot of material like HTML elements, tags, and attributes. We also discussed CSS properties and how to style a responsive web page using these properties. There is much more to learn about web page development, so check out these resources if you want to keep learning:
HTML: https://www.w3schools.com/html/default.asp
CSS: https://www.w3schools.com/css/default.asp
Responsive Web Design: https://www.w3schools.com/html/html_responsive.asp
