### How does a browser render HTML, CSS, and JS to DOM? What is the mechanism behind it?

The rendering of HTML, CSS, and JavaScript in a web browser involves several steps and is a complex process. 
1. HTML Parsing:
  The browser starts by fetching the HTML document from the web server. It then parses the HTML document to create a Document Object Model (DOM) tree.
  During this parsing, the browser identifies elements and their attributes, creating nodes in the DOM tree accordingly.

1. CSS Parsing and Styling:
  Once the DOM tree is constructed, the browser fetches external CSS files linked in the HTML document.
  It parses the CSS to create a CSS Object Model (CSSOM), which defines the styles, layout, and presentation of elements on the page.

1. Render Tree Construction:
  After determining the computed styles, the browser combines the DOM tree and the CSSOM to create a "render tree" or "layout tree." This tree includes only the elements that are visible to the user and their associated styles.

1. Layout:
  The browser performs layout to determine the size and position of each element in the render tree.
  It calculates how the elements should be displayed on the user's screen, taking into account factors like box dimensions, positioning, margins, and more.

1. Painting:
  The final step involves "painting" the content to the screen. The browser draws each element onto the screen according to the layout and styles.
  This is also known as the "rasterization" process. The browser creates a bitmap image that represents what the user sees on the screen.

1. JavaScript Execution:
  While the above steps are happening, JavaScript code may be encountered and executed. JavaScript can modify the DOM, update styles, and trigger additional layout and painting if needed.

1. Reflow and Repaint:
  Changes to the DOM, CSS, or other page properties may trigger reflows and repaints, which are resource-intensive and should be minimized for optimal performance.

The entire process is iterative and may happen multiple times as the user interacts with the page, causing dynamic changes. 



#### Resources : 
1. https://medium.com/jspoint/how-the-browser-renders-a-web-page-dom-cssom-and-rendering-df10531c9969
1. https://dev.to/anuradha9712/how-does-a-browser-render-a-webpage-2en8
1. https://www.quora.com/How-do-browsers-render-HTML-CSS
