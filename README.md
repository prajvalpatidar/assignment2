Question 1. What is the Box model in CSS? Which CSS properties are a part of it?
ans: A rectangle box is wrapped around every HTML element. The box model is used to determine the height and width of the rectangular box. The CSS Box consists of Width and          height (or in the absence of that, default values and the content inside), padding, borders, margin.
     1) Content:  Actual Content of the box where the text or image placed.
     2) Padding: Area surrounding the content (Space between the border and content).
     3) Border: Area surrounding the padding.
     4) Margin: Area surrounding the border.

Question 2. What are the advantages of using CSS?
ans: The main advantages of CSS are given below:
     1) Separation of content from presentation - CSS provides a way to present the same content in multiple presentation formats in mobile or desktop or laptop.
     2) Easy to maintain - CSS, built effectively can be used to change the look and feel complete by making small changes. To make a global change, simply change the style,         and all elements in all the web pages will be updated automatically.
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
 
Question 5. Can you name the four types of @media properties?
ans: The four types of @media properties are:
     All → It’s the default property. Used for all media-type devices.
     Screen → Used for computer screen, mobile screen.
     Print → Used for printers.
     Speech → Used for screen readers.

Question 6. What is the grid system?
ans: CSS Grid Layout is the most powerful layout system available in CSS. It is said to be a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox      which is largely a 1-dimensional system.

Question 7. What are the different ways to hide the element using CSS?
ans: Using display property(display: none). It’s not available for screen readers. The element will not exist in the DOM if display: none is used.
     Using visibility property(visibility: hidden), will take up the space of the element. It will be available to screen reader users. The element will actually be present        in the DOM, but not shown on the screen.
     Using position property (position: absolute). Make it available outside the screen.

Question 8. What does the :root pseudo-class refer to?
ans: The root selector allows you to target the highest-level “parent” element in the DOM, or document tree. It is defined in the CSS Selectors Level 3 specification.

Question 9. What does Accessibility (a11y) mean?
ans: Accessibility refers to how software or hardware combinations are designed to make a system accessible to persons with disabilities, such as visual impairment, hearing        loss, or limited dexterity.
     For example, a website developed with accessibility in mind might have text-to-speech capabilities. In the USA public websites have to have accessible compliance. It’s        defined in 508 compliance. It gives the guidelines and best practices for all website users that should be met with key areas of accessibility.

Question 10. How do I restore the default value of a property?
ans: The keyword initial can be used to reset it to its default value.

Question 11. Difference between CSS grid vs flexbox?
ans: CSS Grid Layout is a two-dimensional system, meaning it can handle both columns and rows. Grid layout is intended for larger-scale layouts which aren’t linear in design.
     Flexbox is largely a one-dimensional system (either in a column or a row). Flexbox layout is most appropriate to the components of an application.


Question 12. What is the difference between CSS variables and preprocessor(SASS, LESS, Stylus) variables?
ans: CSS variables can be used without the need of the preprocessor. Currently, all the major browsers support the CSS variables. 
     CSS variable cascade. But the preprocessor variables don’t cascade. 
     CSS variable can be accessed and manipulated javascript.


Question 13. What does * { box-sizing: border-box; } do? What are its advantages?
ans: It makes every element in the document include the padding and border in the element’s inner dimension for the height and width computation.  In box-sizing: border-box,      The height of an element is now calculated by the content's height + vertical padding + vertical border width.
     The width of an element is now calculated by the content's width + horizontal padding + horizontal border width.

Question 14. What is specificity? How to calculate specificity?
ans: A process of determining which CSS rule will be applied to an element. It actually determines which rules will take precedence. Inline style usually wins then ID then        the class value (or pseudo-class or attribute selector), the universal selector (*) has no specificity. ID selectors have a higher specificity than attribute selectors.

Question 15. What are the advantages of using translate() instead of absolute position?
ans: Translate() does not cause the browser to trigger repaint and layout and instead only acts on the compositor. The absolute position triggers the repaint or DOM reflow.        So, translate() gives the better performance.

Question 16. What is CSS specificity?
Ans: CSS specificity is a score or rank that decides which style declaration has to be used to an element. (*) this universal selector has low specificity while ID selectors      have high specificity.
     There are four categories in CSS which authorize the specificity level of the selector.
     Inline style
     IDs
     Classes, Attributes, and pseudo-classes.
     Elements and pseudo-elements.

Question 17. How can we calculate specificity?
Ans: To calculate specificity we will start with 0, then we have to add 1000 for each ID and we have to add 10 to the attributes, classes or pseudo-classes with each element      name or pseudo-element and later we have to add 1 to them.

Question 18. What are gradients in CSS?
Ans : It is a property of CSS which allows you to display a smooth transformation between two or more than two specified colors.
      There are two types of gradients that are present in CSS. They are:
      Linear Gradient
      Radial Gradient
     
Question 19. What is CSS flexbox?
Ans: It allows you to design a flexible responsive layout structure without using any float or positioning property of CSS. To use CSS flexbox you need to define a flex           container initially.
    Example:
    <!DOCTYPE html>
    <html>
    <head>

    <style>
    .flex-container {
     display: flex;
     background-color: #f4b042;
     }
     .flex-container > div {
     background-color: #d60a33;
     margin: 10px;
     padding: 20px;
     font-size: 30px;
     }
     </style>
     </head>
     <body>
     <div class="flex-container">
       <div>1</div>
       <div>2</div>
      <div>3</div> 
     </div>
     <p> Example of  <em>flex</em>box.</p>
     </body>
     </html>
    
Question 19. Write all the properties of the flexbox?
Ans: There are several properties of the flexbox that are used in the HTML webpage.
     They are:
     1) flex-direction
     2) flex-wrap
     3) flex-flow
     4) justify-content
     5) align-items
     6) align-content   
     
Question 20. What is the use of the Box Model in CSS?
Ans: In CSS, the box model is a box that binds all the HTML elements and it includes features like margins, border, padding, and the actual content.
     By using a box model we will get the authority to add the borders all around the elements and we can also define the space between the elements.

Question 21. How can we add icons to the web page?
Ans: We can add icons to the HTML webpage by using an icon library like font-awesome.
     We have to add the name of the given icon class to any inline HTML element. (<i> or <span>) . Icons in the icon libraries are scalable vectors that can be customized          with CSS.

Question 22. What is a CSS pseudo-class?
Ans: It is a class that is used to define a special state of an HTML element.
     This class can be used by styling an element when a user snooped over it and also it can style an HTML element when it gets the focus.
     selector:pseudo-class {
     property:value;
     }

Question 23. Explain the concept of pseudo-elements in CSS.
Ans: It is a feature of CSS which is used to style the given parts of an element.
     For Example, we can style the first letter or line of an HTML element.
     selector::pseudo-element {
     property:value;
     }
     
Question 24. What is CSS opacity?
Ans: It is the property that elaborates on the transparency of an element.
     By this property, we can transparent the image that can take the values from 0.0-1.0. If the value is lower, then the image is more transparent. IE8 and earlier versions      of the browser can take the values from 0-100.
     
     img {
     opacity: 0.6;
     filter: alpha(opacity=60); /* For IE8 and earlier */}

Question 25. Write all the position states used in CSS.
Ans: In CSS, there are four position states as stated below:
     Static(default)
     Relative
     Fixed
     Absolute

Question 26. What are navigation bars in CSS?
Ans: By using navigation bars we can make an ordinary HTML page into a user-specific and more dynamic web page. Basically, it is a list of links, hence use of <ul> and <li>        elements makes the perfect sense.

     ul {
     list-style-type: none;
     margin: 0;
     padding: 0;
     }

Question 27. What are the differences between relative and absolute in CSS?
Ans: The main difference between relative and absolute is that “relative” is used for the same tag in CSS and it means that if we write the left:10px then the padding will        shift to 10px in the left while absolute is totally relative to the non-static parent.
     It means, if we write left:10px then the result will be 10px far from the left edge of the parent element.
     
Question 28. What are the differences between relative and absolute in CSS?
Ans: The main difference between relative and absolute is that “relative” is used for the same tag in CSS and it means that if we write the left:10px then the padding will        shift to 10px in the left while absolute is totally relative to the non-static parent.
     It means, if we write left:10px then the result will be 10px far from the left edge of the parent element.

Question 29. Define ‘important’ declarations used in CSS?.
Ans: Important declarations are defined as that declaration which is having more importance than the normal declaration.
     While executing, these declarations override the declaration which is having less importance.
     For example, if there are two users having an important declaration then one of the declarations will override the declaration of another user.
     For Example:
     Body {background: #FF00FF !important; color: blue}
     In this body, background has more weight than the color.

Question 30. Define different cascading methods that can be used inside the cascading order?.
Answer: Cascading order is itself a sorting method that allows many other different sorting methods:

          a) Sort by origin: There are some rules which can provide an alternate way defined as:
          The normal weight of the style sheet of a particular provider will be overridden by the increased weight of the user’s style sheet.
          Stylesheet rules of a particular user will be overridden by the normal width of the provider’s style sheet.
          b) Sort by selector’s specificity: Less specific selector is been overridden by the more specific selector.
          For example, A contextual selector is less specific in comparison to the ID selector which is a more specific one and with that contextual selector is been                    overridden by the ID selector.
          c) Sort by order specified: This comes in the scenario when the two selectors are of same weight and the other properties than the specification which will be seen            for overriding.
           Example:
               All other styles will be seen overridden if the style attribute is used for inline style.
               And also, if the link element is used for external style, then it will override the imported style.
      

