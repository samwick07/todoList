# JS Fundamentals III - To-Do List

## 1 Fundamentals To-Do List

### This project will evaluate your ability to implement a JavaScript driven to-do list. The goal of this workshop is not to finish quickly, but rather to do the best you can so we can gauge where everyone in the class is at and how well you're absorbing the material. Take your time and don't stress out!

You will be:

- Using git to create and manage a repository
- Implementing a to-do list based on requirements
- Utilizing HTML to provide structure for the webpage
- Utilizing JavaScript to make the page dynamic
- Utilizing CSS to style the page
- Submitting the project:
- Submit a link to your repository below.
- Project Instructions
- For this webpage you will be implementing a to-do list application. Provided are the setup instructions, requirements, and a list of stretch goals to be - completed if time allows.

### Create your repository
Begin by creating a new public repository in Github and adding the necessary files:

1. Log in to Github and create a new public repository. Why public? So the instructors can see it. Generally your will not want public repositories unless you want your code to be open source: ![Alt](https://s3.us-west-2.amazonaws.com/forge-production.galvanize.com/content/1177c721746752da7aab9e518e3f8571.png "New Public Repo")
2. Why wait? Submit your repo's HTTP link at the bottom of this lesson.
3. After creating the repo, clone the repository onto your computer using the ssh link:
```
`git clone <your repo ssh address>`
```
4. Navigate into your project folder to create your main HTML file index.html:
`cd <your project>`
touch index.html
Create your css file:
touch style.css
Create your js file.
touch index.js
And if you didn't create one by default when making your repo, add a README file. The .md stands for markdown:
touch README.md
As you go through your project, you should be making commits to your project and periodically pushing your commits to the remote. To make a commit for the files we just created you can run:
git add *
git commit -m 'created html, css, and js files'
Push in the following way, you should be able to see the files on GitHub after this step (pending a page refresh):
git push
Begin writing your HTML file
Next we will add the starter code for our HTML file and link it to our CSS and JS files.

Open up your project folder in VS Code then open the currently empty index.html file.
VS Code has some snippets added to it by default thanks to the Emmet package. If you start typing html, you should see a window appear with snippet suggestions. Selecting html:5 from the list will fill in the basic structure for your page. If it doesn't work, just copy/paste the code below into your index.html file:


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>

</body>
</html>


Let's link our JS and CSS files to the HTML file. Within the <head> tag, add a link element to link the CSS file:
<head>
  ...
  <link rel="stylesheet" href="./style.css">
</head>
Great, now when the browser loads our page, it will refer to our css file for all of the styling.
Next we need to include our JavaScript file, except this time we'll add a script element inside the <body> tag:
<body>
  ...
  <script src="./index.js"></script> 
</body>  
But we don't have a blank page when testing, let's add a header within our body tags, so we can actually see something when we load the page:
<body>
  <h1>My page</h1>
  ...
Adding JavaScript
Let's make sure our js file is included. Add a line to do some logging into your index.js file:

console.log('My code is running');
As soon as our page displays and assuming everything is hooked up correctly, the browser will run whatever code we have placed in our index.js file. In this case, our code will add some logging to the browser's developer console.

Adding CSS
To check that css is being included we can add some quick styling by changing the text color of headers from the default black to something else. We can do that by adding the following to our style.css file:

h1 { 
  color: purple;
}
Opening your page and verifying setup
Start by making sure you have saved all of your files. You will forget a million times, just like the instructor writing this document...

In VS Code, right-click on the index.html filename and select Copy Path. Paste this into the navigation bar of your browser (where you would normally type google.com).

If we have linked everything correctly we should be able to see a few things, namely:

We can see the 'My page' header text
HTML works
The color of the header is purple
CSS file is linked correctly
Opening up the developer console and viewing the console output should show our message of 'My code is running'
JS file is linked and running.
To see the logging, open up the developer console by right-clicking on your header and choosing Inspect. From there click on the console tab. You may need to refresh your page to see the logging.

If you find that something isn't working as expected, start by reviewing the instructions again, then ask folks in your group, then reach out for further assistance. As a general rule, spending longer than 15 minutes on a problem without progress is a sign you should seek help.

As you continue developing, refresh your page to see your updates. Have fun and good luck!

Requirements
In this application you will create a to-do list application that can do the following:
Users should be able to view all of the to-do tasks
Users should be able to add a to-do to the list of to-do tasks
Users should be able to remove to-do's, this could be either deletion or crossing out
The page should be aesthetically pleasing (aka be styled)
For now do not worry that your page resets during a refresh, making that work is a stretch goal.

If you don't know where to begin, here's the recommended path:

Start by adding the HTML code. This is like the skeleton of the page, so add a title, list, form, input, buttons, etc...
Add your JavaScript
Create a variable that will hold your to-do list items.
Add a function that takes in a string as input and adds it to the to-do list.
Add an event handler to populate an HTML element with your to-do list when the user clicks the appropriate button.
Etc... break down the big problems into baby steps and solve them systematically. Test as you go.
With the main functionality in place, style your HTML elements using CSS. Make use of the developer console for testing styling.
Finished with the main objectives? Continue on to the stretch goals to make your application even better.
Stretch goals
Add some instructions to your README.md file around what your application is, how to run it, and how to use it.
Make the list persist through a refresh of the page by using local storage to store to-do's
Archive completed tasks in a viewable location on screen