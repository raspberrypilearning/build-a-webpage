## Build and test

Now it's time to build your web page. 

**Tip:** Plan your project so you will be able to create a basic web page in the time you have available and then upgrade the project if you have time left. 

![A screenshote of the 'triple filter test' example webpage.](images/step-three.PNG)

**Tip:** Remember to test your project each time you add something. It is much easier to find and fix bugs before you make more changes.

--- task ---

You have built up some really useful skills. Here is a reminder to help you make your web page: 

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

Choose fonts to use on your web page:

[[[included-fonts]]]

[[[web-fonts]]]

[[[google-fonts]]]

You can use placeholder text while you work on your layout:

[[[add-placeholder-text]]]

Insert text elements:

[[[web-ordered-list]]]

[[[web-unordered-list]]]

[[[full-width-quote]]]

[[[web-large-text-tiles]]]

Style your text:

[web-headers-large-text]

[[[web-center-text]]]

[[[web-strong-em]]]


### Images

Insert an image from the starter project library:

[[[trinket-image-library]]]

[[[web-alt-text]]]

Use an emoji as an image:

[[[choose-an-emoji]]]

[[[huge-emoji]]]

Add a background image:

[[[web-background-image]]]

[[[add-transparency]]]

Tip: You can style your images with rounded corners or borders:

[[[rounded-corners]]]

[[[web-borders]]]

<mark>Add box-shadow</mark>


### Animations

Create web flip cards.

[[[web-flip-cards]]]

Use animations to change the appearance or position of elements on your page over time:

[[[web-starter-animations]]]

[[[web-customise-animations]]]

### More style

Add more style to any elements on your web page:

[[[rounded-corners]]]

[[[web-borders]]]

[[[add-a-gradient]]]

You can create your own class to make a new style:

[[[web-add-class]]]

--- /task ---

--- task ---

**Test:** Show someone else your project and get their feedback. Do you want make any changes to your web page? 

[[[trinket-publish-project]]]

[[[check-accessibility]]]

--- /task ---

--- task ---

**Debug:** You might find some bugs in your HTML or CSS that you need to fix. Here are some common bugs.

**My webpage isn't displaying correctly**

[[[incorrect-tags]]]

mismatched-tags

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

