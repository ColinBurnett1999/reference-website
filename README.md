# reference-website
1. Naming convention for all filenames, paths and folders
- The naming conventions for all filenames should be lowercase, no spaces and dashes are fine. Folder naming convention should be similar to filenames. For paths, the folders, assets and files should be inside the root folder so they can be easily linked inside any .html files
    `index.html`
    2. Best practices for commit messages
    - Commit messages should be descriptive and not use the same terminology too often. Each commit should have a distinct name and commit messages should be a 5 words to a sentence long. Commit messages should also not be in all caps.
    3. What is HTML?
    - HTML stands for "Hypertext Markup Language" and is the code language used to create the contents of websites.
    4. Proper Syntax for HTML Elements
    - HTML elements are mainly comprised of block elements and inline elements, which are enclosed within opening and closing tags, such as
    <p>paragraph</p>. Certain elements such as <img> do not require a closing tag and instead are just a tag with the content specified inside.
    5. Explain or demonstrate commonly used HTML tags/elements:
    - Headings, created with <h1> through <h6>, create text at various set sizes, usually to mark different sections of the page.
    - Paragraphs are created with <p>, the tag designates text in a small body font to appear on the page.
    - Lists, created with <ul>, <ol> or <dl> create a row of text for each item in the list, which can be marked with dashes, dots, numbers, etc. 
    - Links are created with <a>, being clickable text that takes the user to another page, file, etc.
    - Images are placed with <img>, and are displayed on the page or within another element via a link.
     - Figures are elements used to wrap an image along with a caption tag, created with <figure>.
     - Quotes are marked with <q>, typically within another element.
     - Block quotes, created with <blockquote>, are their own text element on a page.
     - Citations are created with <cite>, and show the source of a quote.
     - <em> marks text as emphasized, making it bolder.
     - <strong> emphasizes text even more them <em>.
     - <b> marks a keyword.
     - <i> is used to mark another language, title or technical term.
     - <small> shrinks text, making it harder to read but also take up less space on the page.
     6. Explain block Elements and also explain the list of block elements and why they are used from below:
     - Block elements are elements that take up the entire row of the rows they occupy, and are as tall as their contents.
     - 
     - <head> is used to designate the header of a page, which lets it stay at the top regardless of how the page's content is adjusted.
     - The body tag is used to designate the main content of the page.
     - Headers are marked with <header>, designating the section which appears at the top of the page.
     - The navigation element (<nav>) is a block element containing links to navigate to other pages of the website.
     - The main tag, <main>, designates the main contents of the page and tells the browser where it is.
     - The section tag, <section>, designates a section of the page's content allowing the browser to recognize it. It also allows for easy navigation to that section.
     - <article> marks on article on the page, allowing hte browser to recognize its location and for quick navigation to it if given an ID.
     - The <div> tag marks a division in the page, acting as a container for elements.
     - <aside> is an element used to contain content which is only somewhat relevant to the main content of the page.
     - <footer> is used to contain elements at the bottom of the page.
     - <span> is an inline container for content with no specific purpose.
     - <small> is used to designate smaller text for things like copyright tags, descriptions for images/videos, etc.
     7.Explain why accessibility is important and also explain the accessibility properties like:
     - Accessibility is important because being able to use the internet is a crucial part of modern day-to-day life. Not making websites with those with impairments and disabilities in mind would prevent many people from using it and be unfair.
     - Landmark roles are a set of roles that allow those with screen readers to jump from section to section of the page.
     - Aria labels are labels that can be read by screen readers for those with disabilities that prevent them from reading the contents of the page normally.
     - Image alternative texts are text specified for an image which is read by screen readers.
     8. What is CSS and how can we implement CSS to our html file?
     - CSS stands for "cascading style sheet" and is a file that allows us to format various aspects of our page's appearance such as fonts, the background colour, etc.
     A CSS file is linked to the html file like so:
     <link rel="stylesheet" href="css/style.css">
     9. What is the difference between CSS property and value?
     - The property is the aspect of and way you want to style part of your page. The value is the number, color, etc. given for how the element is styled.
     h1{color: red;} 
     In the above example, "color" is the property while "red" is the value.
     10. Why do we use border-box property in CSS?
     - To prevent different elements from overlapping or being too close and looking cluttered. 
     11. Explain different type of ways we can add spacing to an element
     - Padding, Border and Margin are all aspects of the box that can be adjusted to space a box. Padding pushes the edge of the box away from the content, border creates a stroke around the box which stops the background color from being behind the box and making it blend in, and margin forces other elements away from the border.
     12. What is the main difference between margin and padding?
     - Padding increases the size of the box, while margin pushes other elements away from it.
     13. What are different types of display properties?
     - "inline" allows other elements on the same line, "block" forces other elements onto different lines, "inline-block" is the same as inline but allows control of the height and width values and "none" removes the element from the page.
     14. Write a brief explanation of flexbox property
     - Flexbox allows you to more elaborately arrange elements on a page to create different layouts.
     15. What are different types of flexbox properties and what is the major difference between them?
     - Flex and inline-flex are the different types of flexboxes, with one taking up its own lines and one allowing other elements on the same lines, just like block and inline elements.
     16. Explain with code the use of flexbox property on a parent element and also explain the sub properties you might need for the flexbox property.
     - Flexbox is applied to the parent element with code like this:
     article{
      display: flex; 
     }
     but affects the children of the parent element. Sub-properties such as
     "flex-start", "flex-end", "center", "space-around", and so on are needed to specify how things will be arranged.
     17. Write a code example on how you will use a flexbox property on a parent element with sub properties.
     - nav {
      display: flex;
      flex-direction: column;
      justify-content: right;
      align-content: space-around;
     }
     18. What is CSS grid property?
     - A property that arranges elements across a set of horizontal and vertical lines which can be adjusted and arranged in various ways.
     19. Write the parent and two sub-properties used for CSS Grid Property.
     - .grid-container {
      grid-template-rows: auto;
      align-self: center;
     }
     20. What is the difference between display: flex and display: grid?
     - display: flex; arranges the items into a column or row, while display: grid; arranges items into multiple columns and rows which are all adjacent unless specified otherwise.
     21. What sub-property we use to divide elements in CSS Grid properties?
     - space-around, space-evenly & space-between when used under "align-self" or "justify-self" will divide the grid into either columns or rows with gaps between them.
     22. What unit we use to fractionally divide the element width in CSS Grid property and what are others unit we can use alternatively? (Write a code example)
     - fr units allow you to determine sizes and spacing via fractions of the remaining space, like so:
     grid-template-rows: 2fr;
     - Alternatively, "auto" will automatically space elements similarly to fr units.
     23. What is the area property in CSS grid we use for the child elements?
     - "child-of-grid-item"
     24. Which sub-property of display grid you can use to prevent displaying empty columns. Write a code example of that property.
     - "auto-fit" will expand columns to fit the space rather than leaving empty ones. You would write it like so:
     grid-template-columns:
     repeat(auto-fit(2fr));
     25. Explain the steps to add google fonts to your CSS file and how will you link it to the html file.
     - Step 1: Go to fonts.google.com
     - Step 2: Find the font you wnat to use
     - Step 3: Select the variations you want
     - Step 4: Open your "selected families"
     - Step 5: Click the <link> option and copy the link onto your clipboard.
     - Step 6: Paste the link(s) under your <head> section in your HTML file. You can now use the fonts you linked to style your text in CSS.