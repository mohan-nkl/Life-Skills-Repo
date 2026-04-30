# Browser Rendering: How HTML, CSS, and JavaScript Become a Web Page

## Introduction
When we open a website in a browser, it does not directly show the page. It first reads the HTML, CSS, and JavaScript, and then converts them step by step into something we can see on the screen. This process is called browser rendering. Understanding this helps us write better and more efficient web applications.

## Rendering Process

1. HTML Parsing and DOM Creation  
   The browser reads the HTML file and converts it into a structure called the DOM (Document Object Model).  
   You can think of this as a tree that represents all elements like headings, paragraphs, and buttons.

2. CSS Parsing and CSSOM Creation  
   The browser then reads the CSS and creates another structure called the CSSOM.  
   This contains all the styling information like colors, sizes, and layouts.

3. Render Tree Construction  
   The DOM and CSSOM are combined to form the Render Tree.  
   This tree only includes the elements that will actually be visible on the screen along with their styles.

4. Layout  
   In this step, the browser calculates where each element should be placed and how much space it should take.  
   This decides the position and size of every element.

5. Painting  
   Finally, the browser draws everything on the screen as pixels.  
   This is the step where we actually see the webpage.

6. JavaScript Execution  
   JavaScript runs alongside this process and can modify both the DOM and CSS.  
   If changes are made, the browser may need to repeat layout and painting again.

## Key Points

* HTML defines the structure of the page  
* CSS defines how the page looks  
* DOM represents structure inside the browser  
* CSSOM represents styling rules  
* Render Tree combines structure and style  
* Layout decides position and size  
* Painting displays the final output  

## Conclusion
Browser rendering is a step-by-step process where the browser builds the page from code and displays it on the screen. By understanding how DOM, CSSOM, and rendering work together, we can write cleaner code and avoid unnecessary performance issues.

## References

* https://developer.mozilla.org/en-US/docs/Web/Performance/How_browsers_work
* https://web.dev/critical-rendering-path/
* https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model