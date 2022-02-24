# Semantic Markup Refactor

This is my first homework assignment for my full stack front-end development bootcamp.

The purpose of this assignment is to learn about semantic HTML. The goal was to refactor an existing site to make it more accessible using semantic HTML.

Through this assignment I learned the importance of semantic HTML and practiced navigating refactoring HTML without inferring with the existing styling.

---
## Website

### [Navigate to the live website](https://struelensc.github.io/semantic_markup_refactor/)

The follow image shows the web application's appearance:

![Mockup for Website](/assets/Mockup.png)

---
## Changes Made

Changes were made to add semantic HTML to meet accessibility standards, to consolidate and organize the CSS to logically stand beside the HTML, and to fix any existing bugs. Both the CSS and HTML were also commented and formatted to be more readable and maintainable.

### The below was changed to meet accessibility standards by changing non-semantic HTML elements to semantic HTML elements.
- Gave all the photos `<alt>` tags.
- Changed the `<div>` with the class header to a `<header>` tag.
- Changed the `<div>` containing the list for the navigation links in the header to a `<nav>` tag.
- Changed the `<div>` tag containing the content to a `<main>` tag as this content is the main content for the page.
- Changed the `<div>` tags containing 'Search Engine Optimization', 'Online Reputation Management', and 'Social Media Marketing' to `<section>` tags as these are separate sections of the main content.
- Changed the `<div>` tag containing the benefits to an `<aside>` tag as this information lays to the side and compliments the main content. 
- Changed the `<div>` tags containing 'Lead Generation', 'Brand Awareness', and 'Cost Management' to `<section>` tags as these are separate sections of the benefit information.
- Changed the `<div>` containing the footer to a `<footer>` tag.
- Changed the `<div>` containing the hero class to a `<figure>` tag. Added a `<aria-label>` attribute.
    - I couldn't add an alt attribute to this photo as it was being pulled by the CSS file and not the HTML file, so an aria-label attribute was used to provide accessibility to this photo.

### The below was changed to consolidate the CSS and to organize it so it is structured logically alongside the HTML.
- Changed the class for the sections in the content container to "content-section" and consolidated the CSS for these elements. This was done because the styling was the same for each of these sections. The positioning of the CSS for these elements was also changed to logically follow the HTML structure.
- Changed the classes of the sections in the benefit aside to ids and added the class "benefit-section" to each section. Then the CSS was consolidated for these elements. This was done because the styling was the same for each of these sections. I left ids if unique styling was ever desired.

### Additional changes listed below.
- Added comments to CSS file.
- The id was missing for the "search-engine-optimization" section in the main content container for the navigation link to call when it was clicked. I added the corresponding id to fix this bug.
- Changed the title to be more descriptive.