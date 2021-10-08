Question 1. What is the Box model in CSS? Which CSS properties are a part of it?
ans: A rectangle box is wrapped around every HTML element. The box model is used to determine the height and width of the rectangular box. The CSS Box consists of Width and          height (or in the absence of that, default values and the content inside), padding, borders, margin.
     1) Content:  Actual Content of the box where the text or image placed.
     2) Padding: Area surrounding the content (Space between the border and content).
     3) Border: Area surrounding the padding.
     4) Margin: Area surrounding the border.

Question 2. What are the advantages of using CSS?
ans: The main advantages of CSS are given below:
     1) Separation of content from presentation - CSS provides a way to present the same content in multiple presentation formats in mobile or desktop or laptop.
     2) Easy to maintain - CSS, built effectively can be used to change the look and feel complete by making small changes. To make a global change, simply change the style, and         all elements in all the web pages will be updated automatically.
     3) Bandwidth - Used effectively, the style sheets will be stored in the browser cache and they can be used on multiple pages, without having to download again.

Question 3. What are the limitations of CSS?
ans: Disadvantages of CSS are given below:
     1) Browser Compatibility: Some style selectors are supported and some are not. We have to determine which style is supported or not using the @support selector).
     2) Cross Browser issue: Some selectors behave differently in a different browser).
     3) There is no parent selector: Currently, Using CSS, you can’t select a parent tag.

Question 4. How to include CSS in the webpage?
ans: There are different ways to include a CSS in a webpage, 
     1 -External Style Sheet: An external file linked to your HTML document: Using link tag, we can link the style sheet to the HTML page.
                                 <link rel="stylesheet" type="text/css" href="mystyles.css" />
     2 -Embed CSS with a style tag: A set of CSS styles included within your HTML page.
                                 <style type="text/css">
                                 /*Add style rules here*/
                                 </style>
        Add your CSS rules between the opening and closing style tags and write your CSS exactly the same way as you do in stand-alone stylesheet files.
     3 -Add inline styles to HTML elements(CSS rules applied directly within an HTML tag.): Style can be added directly to the HTML element using a style tag.
                                 <h2 style="color:red;background:black">Inline Style</h2>
     4 -Import a stylesheet file (An external file imported into another CSS file): Another way to add CSS is by using the @import rule. This is to add a new CSS file within         CSS itself.
                                  @import "path/to/style.css";
     5. What are the different types of Selectors in CSS?
 
    
