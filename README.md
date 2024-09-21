# Web Dev Starter Code

## Overview

This project is mainly to ensure good practice and accessibility while creating a new page.

## Compile and Run

- Open the index.html file
- Run your html preferred server to view the html file.
- i.e. VSCode plugin, IntelliJ IDE, etc.

## Sources and Credits

- Professor Panter: starter code and repo
- Aria-label: <https://www.w3schools.com/accessibility/accessibility_labels.php>

## Accessibility Lab Answers

### Color

The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors?

- I've forgotten the init

### Semantic HTML

1. The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.

- For the most part everything here seemed to be working! Except the show/hide comment button not being detected by keyboard navigation.

2. Can you update the article text to make it easier for screen reader users to navigate?

- There are a number of things that needed to be updated that would leave screen readers in a bind. Such as, no header tags, div tags that act in place of the appropriate tags, etc.

3. The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.
   Note: You'll need to update the CSS rule selectors that style the tags to their proper equivalents for the semantic headings. Once you add paragraph elements, you'll notice the styling looks better.

- As mentioned previously the div tag can be skipped by the screen readers so having the proper `<nav>` tag can be a great help here.

### The Images

The images are currently inaccessible to screen reader users. Can you fix this?

- For screen readers, it is important that the alt text depicts what the image is.

### The Audio Player

1. The <audio> player isn't accessible to hearing impaired (deaf) people — can you add some kind of accessible alternative for these users?

- By adding an audio transcript.

2. The <audio> player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio?

- We provide the file for download if the browser does not support HTML audio.

### The Forms

1. The <input> element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers?

- An aria-label is appropriate if the content surrounding the element is informative enough for visual user and doesn't necessarily need to be visible. This way we can ensure we still have a label for screen readers.

2. The two <input> elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this? Note that you'll need to update some of the CSS rule as well.

- We can use proper label tags to associate it with the corresponding form input.

### The Show/Hide Comment Control

The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key?

Making the show/hide comment control button a proper button instead of a clickable div makes this more keyboard-accessbile and allows for control the return key.

### The Table

The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem?

- Adding a caption or summary is good to explain the expected content of the table.

- Explicitly specifying table headers in the appropriate sections are important. As well as defining what scope are for (col, row). Only then does the table proceed to the standard table data.

- The table data itself could associate itself with the appropriate headers using the `headers` attribute.

