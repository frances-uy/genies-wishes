# Genie's Wishes
This project was created for the Spring 2024 [ICSpark Program](https://icspark.github.io/)

## Objective

Use HTML Links, Images, Headers and correctly specify the file paths to develop a choose-your-destiny story.

## Prerequisites

To complete this project, students should have the following:

* Basic understanding of HTML structures and attributes.
* Basic understanding of CSS (Selectors, Basic Properties like Width and Height)

## Concepts
### HTML and CSS Structures and Attributes
| HTML      | Description                                                                      | 
|-----------|----------------------------------------------------------------------------------|
| HTML      | H yper T ext M arkup L anguage used to create the structure of web pages.        | 
| element   | An element is an individual part, or a building block, of a web page.            | 
| attribute | A modifier of an element.                                                        | 
| div       | A container of an element.                                                       | 
| img       | An image element.                                                                | 
| a         | A link element.                                                                  | 
| href      | An attribute used to specify the link destination.                               | 
| link      | A link tag that links external style sheets to your HTML page.                   |
| id        | A unique attribute on an element used for targeting in CSS.                      | 
| class     | An attribute that can be applied to multiple elements used for targeting in CSS. |

### Absolute vs. Relative File Paths
__File Path__: Description of the location of the file

| File Paths         | Description                                                                                                                                                                   | 
|--------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Absolute File Path | Specifies the complete location of a file or directory in a file system, starting from the root element and including all directories leading to the specific file or folder. | 
| Relative File Path | Specifies the location of a file or directory in relation to the current working directory, not requiring the complete path from the root of the file system.                 | 

## Instructions

_Level of Difficulty: Easy/Medium_

This is an interactive story-telling platform. The primary purpose of the site is to engage users in a narrative where their choices determine the direction and outcome of the story.

### Before Starting

If you are doing this for the first time, it is recommended to download the ``images`` folder from this respository to your local files. This will provide the necessary backgrounds and images to get you started.

You may use the same wishes and scenarios created in the sample, however you are encouraged to come up with your own. Create 3 wishes, and 3 branching scenarios that could happen for each—meaning 9 branching scenarios total.

For each wish and branching scenario, find a special background photo and relating image. These must be in the .jpg format for best compatability. 

_Tip: Images with the .png extension (transparent backgrounds) look nicer against backgrounds!_

### Setting Up Your Repl in Replit

- Import (copy/paste or drag) the ``images`` folder into the Repl project
- Paste this code into the style.css file:

```angular2html
body {
    margin-top: auto;
    text-align: center;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}

img {
    display: block;
    margin: 0 auto;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
}
```

- The ``Webview`` panel to the right of your code will allow you to preview your site. Remember to hit the refresh button to see new changes. You can also pop out your site into a new tab, locally hosted on your browser.
- Create 3 new files called `wish1.html`, `wish2.html`, and `wish3.html`.

### Homepage

1. Navigate to the file called `index.html`, which will be our "homepage". It should have boilerplate code to start off with.
2. If not, copy and paste this boilerplate code:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
    <link rel="stylesheet" href="style.css"> <!-- Link to an external CSS file -->
    <!-- Additional CSS or JavaScript files can be linked here -->
</head>
<body>
    
</body>
</html>

```

3. Edit the title to "Genie's Wishes"
4. Create a ``h1`` header at the top containing "The Mysterious Lamp"
5. Use a ``p`` element to make an introduction to how the genie appears
6. Use a ``img`` element to insert a picture of a genie
7. Use a ``h2`` element containing "Choose a lamp to reveal your fate!"
8. Create a ``<div>`` element with the class name "container"
9. Inside the container `<div>`, create an `<a>` element with an href attribute pointing to wish1.html. This creates a clickable link to the wish1.html page.
        - Inside the `<a>` tag, add an `<img>` tag. Set its src attribute to the image path, and adjust its width if needed.
        -  Repeat that step for the second and third lamps, changing the `href` of each of those respectively.

### Wish Page

1. Add the basic HTML structure
   - Start with the `<!DOCTYPE html>` declaration.
      Add the opening and closing `<html>` tags.
      Within the <html> tags, add the `<head>` and `<body>` sections.
2. Fill in the Head Section
   - Inside the `<head>` tag, add a `<title>` tag with the title "Wealth".
     Link to an external CSS file (named style.css) using the `<link>` tag.
3. Fill in the Body Section
   - Add a `<body>` tag with a class attribute set to "wealth-bkg".
      Inside the body, create headings `(<h1>, <h2>, <h3>)` and paragraph elements as required, with appropriate text content. Assign them the class "wealth-text".
      Include `<img>` tags with src attributes pointing to the respective image files (e.g., "images/wealth-1.jpg").
4. Adding Interactive Buttons
   - Create a `<div>` to contain your buttons.
     Inside the `<div>`, add `<a>` tags, each containing a `<button>` element. Set the href attribute of each `<a>` tag to link to the respective pages (e.g., wish1-button1.html).
     Assign a class (e.g., "button-green") to each button for styling purposes.

Repeat this for the other 2 wishes. 

Here is my final style.css file, however it can be modified to fit your design:

```css
body {
    margin-top: auto;
    text-align: center;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}

img {
    display: block;
    margin: 0 auto;
}

.container {
    display: flex;
    justify-content: center;
    align-items: center;
}

.main-bkg {
    background-image: url(images/silver-bkg.jpg);
    background-size: cover;
}

.wealth-bkg {
    background-image: url(images/wealth-bkg.jpg);
    background-size: cover;
}

.fame-bkg {
    background-image: url(images/fame-bkg.jpg);
    background-size: cover;
}

.knowledge-bkg {
    background-image: url(images/knowledge-bkg.jpg);
    background-size: cover;
}


.wealth-text {
    color: white;
}

.button-green {
    font-size: large;
    color: rgb(27, 95, 21);
}

.button-red {
    font-size: large;
    color: rgb(98, 33, 33);
}
```

### Stretch Goals
- Add alternative options that users can choose within the Wish pages.

