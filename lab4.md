CSS Grid Layout

is a two-dimensional grid-based layout system that aims to do nothing less than completely change the way we design grid-based user interfaces.

CSS has always been used to lay out our web pages, but it’s never done a very good job of it. First, we used tables, then floats, positioning and inline-block, but all of these methods were essentially hacks and left out a lot of important functionality (vertical centering, for instance).

Flexbox helped out, but it’s intended for simpler one-dimensional layouts, not complex two-dimensional ones (Flexbox and Grid actually work very well together).

Grid Container

The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.
Grid Item

The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.
Grid Line

The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.
Grid Track

The space between two adjacent grid lines. You can think of them like the columns or rows of the grid. Here’s the grid track between the second and third row grid lines.
Properties for the Grid Container

Responsive Layouts with CSS Grid
Grid gives us control over how wide or narrow each of the ‘grid cells’ get. This allows us to maintain a sensible aspect ratio to their height The repeat() function takes two arguments, the first will define the number of column tracks and the second, what width the tracks should be.

auto-fill which will create a grid with as many tracks as will fit into the container.

the width of the tracks, The minmax function will create track widths that can be a minimum of 250px wide and a maximum of 1fr. An fr is a ‘fraction unit’, a unit of measurement to define a fraction of the available space of the container. The width of the elements in the row will increase from 250px until the point where another element could potentially fit beside the first.

grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
 (Links to an external site.)display
.container {
  display: grid | inline-grid;
}
 (Links to an external site.)grid-template-columns and grid-template-rows
.container {
  grid-template-columns: 40px 50px auto 50px 40px;
  grid-template-rows: 25% 100px auto;
}
<track-size>: can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)
<line-name> : an arbitrary name of your choosing
 (Links to an external site.)grid-template-areas
.item-a {
  grid-area: header;
}
