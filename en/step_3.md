## Build and test

Now it's time to make your web page. 

Image, gif or video showing what they will achieve by the end of the step. ![](images/image.png)

**Tip:** Remember to test your project each time you add something. It is much easier to find and fix bugs before you make more changes.

--- task ---

You have built up some really useful skills. Here is a reminder to help you make your web page : 

### Colour palette

[[[web-colour-palette-variables]]]

[[[hex-colour-palettes]]]

[[[web-colour-palette]]]

[[[trinket-image-library]]]

[[[colours-from-image]]]

[[[contrast-checker]]]

[[[web-primary-secondary]]]

[[[add-colour-variables]]]

### Structure

[[[full-width-section]]]

[[[side-by-side-section]]]

[[[wrapped-regular-width]]]

[[[three-text-tiles]]]

[[[web-large-text-tiles]]]

[[[text-image-text]]]

[[[wrapped-wide-narrow]]]

[[[full-width-quote]]]

### Fonts and text elements

[[[included-fonts]]]

[[[web-fonts]]]

[[[google-fonts]]]

[[[add-placeholder-text]]]

[[[full-width-quote]]]

[[[web-large-text-tiles]]]

[[[web-center-text]]]

[[[web-strong-em]]]

[[[web-ordered-list]]]

[[[web-unordered-list]]]

[[[full-width-quote]]]

### Images

[[[trinket-image-library]]]

[[[choose-an-emoji]]]

[[[huge-emoji]]]

[[[web-background-image]]]

[[[add-transparency]]]

### Animations

[[[web-flip-cards]]]

[[[web-starter-animations]]]

[[[web-customise-animations]]]

### More style

[[[rounded-corners]]]

[[[web-borders]]]

[[[add-a-gradient]]]

[[[web-add-class]]]

--- /task ---

--- task ---

**Test:** Show someone else your project and get their feedback. Do you want make any changes to your web page? 

--- /task ---

--- task ---

**Debug:** You might find some bugs in your HTML or CSS that you need to fix. Here are some common bugs.

--- collapse ---

---
title: Incorrect tags or properties
---

Carefully check the spelling of your HTML tags, attributes and classes. Incorrect tags can mean that the tag text gets displayed on your web page instead of controlling the layout.

This example incorrectly uses 'image' instead of 'img'! `<img>` is the correct HTML tag. 

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---

    <image class="bordered-box" src="happy.png" alt="An outline of an anime style girl with a happy facial expression."/>

--- /code ---

It is also incorrect to have spaces in tags, this example is incorrect:

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---

< h1>Lorem ipsum</h1>

--- /code ---

--- /collapse ---

--- collapse ---

---
title: Mismatched tags or brackets
---

Make sure that tags with an open and close tag such as `<div>` and `</div>` are correctly matched and nested.

This HTML is incorrect because there is no closing `</div>` tag. 

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---
<section>
<div><p>Lorem ipsum</p>
</section>
--- /code ---

This HTML is incorrect because the `</div>` appears before the closing `</p>` tag.

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---

<div><p>Lorem ipsum</div></p>

--- /code ---

**Tip:** If your HTML is incorrect then sometimes a web browser will work out what you meant. You should still make sure your HTML is correct as incorrect HTML might cause problems later and make make it difficult for screen readers to understand your page. 

--- /collapse ---

--- collapse ---

---
title: My image isn't displayed
---

Check carefully that the name of your image in the `src` property matches the file name. This includes making sure that use of capital letters is the same. 'myimage.png' is *not* the same as 'myimage.PNG'.

This HTML will not display an image saved as 'happy.PNG':

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---

<img src="happy.png" alt="An outline of an anime style girl with a happy facial expression."/>

--- /code ---

--- /collapse ---

--- collapse ---

---
title: My font isn't displayed
---

When you want to use a new google font, you need to make sure you have:

+ Added the `<link>` from google fonts to the `<head>` section of your web page
+ Updated the font variables in `default.css` or the style sheet that you are using for your colour and font palette. 

This example adds the `Bangers` font and uses if for headers and titles, but not for the body:

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---

<!-- Import fonts from Google -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bangers&display=swap" rel="stylesheet">

--- /code ---

--- code ---
---
language: CSS
filename: default.css
line_numbers: false
---

--body-font: 1.1rem Verdana, sans-serif;
--header-font: lighter 3rem 'Bangers', cursive;
--title-font: lighter 2rem 'Bangers', cursive;

--- /code ---

--- /collapse ---

--- collapse ---

---
title: My link to a web page doesn't work
---

Remember that the `<a>` (anchor) tag is used to create a link to another web page (not the 'link' tag which is used to link to resources such as fonts).

Also check that you have the correct web address (url) for the `href` property. 

The part of a web address after the the domain name (such as 'projects.raspberrypi.org'), is case sensitive so you need to make sure capital letters match. 

This example uses correct HTML to link to a web page that will open in a new browser tab:

--- code ---
---
language: HTML
filename: index.html
line_numbers: false
---

<a href="https://projects.raspberrypi.org/en/raspberrypi/web-intro" target="_blank">Make a web page like this!</a>

--- /code ---

--- /collapse ---

You might find a bug not listed here. Can you figure out how to fix it?

We love hearing about your bugs and how you fixed them. Use the feedback button at the bottom of this page if you found a different bug in your project.

--- /task ---

admin type ingredients

[[[trinket-publish-project]]]

[[[check-accessibility]]]