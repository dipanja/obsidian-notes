---
id: "Day 01: Introduction to JavaScript & Setting Up Environments"
aliases: []
tags:
  - javascript
  - javascript/fundamental
---

Date: 14-02-2025

# Introduction to JavaScript & Setting Up Environments

- Basics
- First Script
- Setting
- Things up
- async/defer

"defer" is used in the script tag to execute the script after all the HTML has been rendered properly.
To refer a tab inside the script we use the "id" tag.
Here in the HTML code below we have a div with id="dynamic-paragraph-container".
We can use this id to refer it in the code.

The code below uses defer and script

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Basic HTML with Deferred Script</title>
    <script src="script.js" defer></script>
  </head>
  <body>
    <h1>This is the main heading</h1>
    <p>Some sample text in the paragraph.</p>
    <div id="dynamic-paragraph-container"></div>
  </body>
</html>
```

This is the content of script.js
Here we dynamically add the text "This text is comming form script" in the div that has id="dynamic-paragraph-container".

```JavaScript
// This is the content of script.js
console.log("Script loaded and executed!"); // This will log to the console
document.getElementById('dynamic-paragraph-container').innerText  = "This text is comming from script"
```

### Resources

YouTube: [01: Introduction to JavaScript & Setting Up Environments](https://www.youtube.com/watch?v=t8QXF85YovE&t=0s)

All the topics are here [[40 Days of JavaScript]]
