---
id: "Day 01: Introduction to JavaScript & Setting Up Environments"
aliases: []
tags:
  - JavaScript
---

## Day 01: Introduction to JavaScript & Setting Up Environments

Date: 14-02-2025

### Module: JavaScript Fundamental

- Basics
- First Script
- Setting
- Things up
- async/defer

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

```JavaScript
// This is the content of script.js
console.log("Script loaded and executed!"); // This will log to the console
document.getElementById('dynamic-paragraph-container').innerText  = "This text is comming from script"
```

### Resources

[Day 01: Introduction to JavaScript & Setting Up Environments](https://www.youtube.com/watch?v=t8QXF85YovE&t=0s)
