Templating with Mustache
Mustache can be used for HTML, config files, source code - anything. It works by expanding tags in a template using values provided in a hash or object.

We call it “logic-less” because there are no if statements, else clauses, or for loops.

TAG TYPES
Tags are indicated by the double mustaches. is a tag, as is. In both examples, we’d refer to person as the key or tag key. Let’s talk about the different types of tags.

Variables

The most basic tag type is the variable. A `` tag in a basic template will try to find the name key in the current context. If there is no name key, the parent contexts will be checked recursively. If the top context is reached and the name key is still not found, nothing will be rendered.

All variables are HTML escaped by default. If you want to return unescaped HTML, use the triple mustache: }.

Template:

* 
* 
* 
* }
Hash:

{
  "name": "Chris",
  "company": "<b>GitHub</b>"
}
Output:

* Chris
*
* &lt;b&gt;GitHub&lt;/b&gt;
* <b>GitHub</b>
Install Mustache
Mustache-Express

If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily. To install:

NPM

$ npm install mustache --save
Configure mustache-express in your server.js/app.js/index.js file:



Create a views folder and add some html view templates (e.g. hello.html): 

To use variable passed to HTML like the image bellow



Then in the router configuration, use res.render(TEMPLATE_NAME, JSON_DATA). Example:

res.render('hello', {"name": "Sherlynn"})
Output 

CSS Flexbox


The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

Parent Element (Container)
The flex container becomes flexible by setting the display property to flex:

.flex-container {
  display: flex;
}
The flex container properties are:

flex-direction
flex-wrap
flex-flow
justify-content
align-items
align-content
The flex-direction Property


The flex-direction property defines in which direction the container wants to stack the flex items.

The flex-direction property defines in which direction the container wants to stack the flex items.

.flex-container {
  display: flex;
  flex-direction: column;
}
The column-reverse value stacks the flex items vertically (but from bottom to top):

.flex-container {
  display: flex;
  flex-direction: column-reverse;
}
The row value stacks the flex items horizontally (from left to right):

.flex-container {
  display: flex;
  flex-direction: row;
}
The row-reverse value stacks the flex items horizontally (but from right to left):

.flex-container {
  display: flex;
  flex-direction: row-reverse;
}
The flex-wrap Property


The flex-wrap property specifies whether the flex items should wrap or not.

The wrap value specifies that the flex items will wrap if necessary:

.flex-container {
  display: flex;
  flex-wrap: wrap;
}
The nowrap value specifies that the flex items will not wrap (this is default):

.flex-container {
  display: flex;
  flex-wrap: nowrap;
}
The wrap-reverse value specifies that the flexible items will wrap if necessary, in reverse order:

.flex-container {
  display: flex;
  flex-wrap: wrap-reverse;
}
The flex-flow Property


In the following example we will solve a very common style problem: perfect centering.

SOLUTION: Set both the justify-content and align-items properties to center, and the flex item will be perfectly centered:

