CSS (Cascading Style Sheets) is a stylesheet language used for describing the look and formatting of a document written in HTML.

## CSS Selectors

CSS selectors are used to select elements on a page and apply styles to them. Here are some common CSS selectors:

-   `element`: selects all elements of the specified type
-   `.class`: selects all elements with the specified class
-   `#id`: selects the element with the specified id
-   `element.class`: selects all elements of the specified type with the specified class
-   `element > element`: selects all elements that are direct children of the specified parent element
-   `element + element`: selects all elements that are directly following the specified element
-   `element ~ element`: selects all elements that are preceded by the specified element

## Properties and Values

CSS properties and values are used to define the styles that will be applied to the selected elements. Here are some common CSS properties and values:

-   `color`: sets the color of the text
    -   Example: `color: blue;`
-   `background-color`: sets the background color of an element
    -   Example: `background-color: yellow;`
-   `font-size`: sets the size of the text
    -   Example: `font-size: 16px;`
-   `font-weight`: sets the weight of the text
    -   Example: `font-weight: bold;`
-   `text-align`: sets the alignment of the text
    -   Example: `text-align: center;`
-   `margin`: sets the margin around an element
    -   Example: `margin: 10px;`
-   `padding`: sets the padding within an element
    -   Example: `padding: 10px;`
-   `width`: sets the width of an element
    -   Example: `width: 300px;`
-   `height`: sets the height of an element
    -   Example: `height: 200px;`

## Box Model

The CSS box model describes the rectangular boxes that are generated for elements in the document, and includes the following components:

-   Content: the content of the element, such as text or images
-   Padding: the space within the element and around the content
-   Border: a line that surrounds the padding and content
-   Margin: the space outside the border, between the element and other elements on the page

## CSS Specificity

CSS specificity determines which styles will be applied to an element when there are multiple styles that could apply. In general, the most specific selector wins. Here are some general rules for CSS specificity:

-   An id selector (`#id`) is more specific than a class selector (`.class`) or element selector (`element`)
-   A class selector (`.class`) is more specific than an element selector (`element`)
-   An inline style (`style` attribute on an HTML element) is more specific than a selector in an external stylesheet
-   The last style defined for an element wins, if multiple styles could apply

## Inheritance

CSS inheritance means that styles are passed from parent elements to child elements, unless explicitly overridden. This allows you to set styles on a parent element and have them apply to all of its children.

## CSS Units

CSS units are used to specify lengths, such as font sizes, margins, and widths. Here are some common CSS units:

-   `px`: pixels, a fixed unit of measurement
-   `%`: percentage, relative to the parent element
-   `em`: relative to the font

## CSS Floats

CSS floats are used to float an element to the left or right of its parent element, allowing text to wrap around it. The `float` property is used to specify a float:

-   `float: left;`: floats the element to the left of its parent
-   `float: right;`: floats the element to the right of its parent

## CSS Display

The `display` property is used to control how an element is displayed on the page. Here are some common values for the `display` property:

-   `block`: the element takes up the full width of its parent and creates a new block formatting context
-   `inline`: the element takes up only as much space as necessary and does not create a new block formatting context
-   `inline-block`: the element takes up only as much space as necessary and allows other elements to be on the same line
-   `none`: the element is not displayed on the page

## CSS Positioning

The `position` property is used to control the positioning of an element on the page. Here are some common values for the `position` property:

-   `static`: the default position, the element flows with the other elements on the page
-   `relative`: the element is positioned relative to its normal position
-   `absolute`: the element is positioned relative to its closest positioned ancestor, or the body if there is no positioned ancestor
-   `fixed`: the element is positioned relative to the browser window and does not move when the page is scrolled

## CSS Flexbox

CSS flexbox is a layout model that allows you to control the positioning and sizing of elements within a container. The `display` property is set to `flex` to create a flex container, and the `flex-direction`, `flex-wrap`, and `justify-content` properties are used to control the layout of the flex items.

## CSS Grid

CSS grid is a layout model that allows you to create two-dimensional grids to control the positioning and sizing of elements on the page. The `display` property is set to `grid` to create a grid container, and the `grid-template-columns` and `grid-template-rows` properties are used to define the columns and rows of the grid. The `grid-column` and `grid-row` properties are used to specify which cells elements should be placed in.

## Media Queries

Media queries are used to apply different styles based on the size and characteristics of the device being used to view the page. Media queries use the `@media` rule to specify styles that should only be applied if certain conditions are met, such as the screen width being greater than a certain size.

Example:
```css
@media (min-width: 700px) {
  body {
    background-color: lightblue;
  }
}
	```
This media query applies a light blue background color to the body if the screen width is 700 pixels or wider.



## CSS Box Model

The CSS box model defines how elements on a page are sized and positioned. It consists of the content area, padding, borders, and margins. By default, the size of an element is defined by its width and height properties, and the position of an element is defined by its top, right, bottom, and left properties.

## CSS Text

The CSS text properties are used to control the appearance of text on a page. Here are some common CSS text properties:

-   `font-family`: specifies the font family to be used for the text
-   `font-size`: specifies the size of the text
-   `color`: specifies the color of the text
-   `text-align`: specifies the horizontal alignment of the text
-   `text-decoration`: adds a line to the text, such as an underline or strike-through
-   `line-height`: specifies the height of a line of text
-   `letter-spacing`: specifies the amount of space between characters in a text
-   `word-spacing`: specifies the amount of space between words in a text

## CSS Backgrounds

The CSS background properties are used to control the background of an element. Here are some common CSS background properties:

-   `background-color`: specifies the background color of an element
-   `background-image`: specifies an image to be used as the background of an element
-   `background-repeat`: specifies if the background image should be repeated and how
-   `background-position`: specifies the position of the background image
-   `background-size`: specifies the size of the background image

## CSS Transitions

CSS transitions are used to animate changes in styles over time. The `transition` property is used to specify the transition effect, and the `transition-property`, `transition-duration`, `transition-timing-function`, and `transition-delay` properties are used to control the details of the transition.

Example:
```css
button {
  transition: background-color 0.5s ease-in-out;
}

button:hover {
  background-color: lightblue;
}
	```

In this example, the background color of the button will transition to light blue over 0.5 seconds with an ease-in-out timing function when the button is hovered over.

## CSS Pseudo-Classes Cheat Sheet

CSS pseudo-classes are used to select elements based on their state or position. Here is a comprehensive list of CSS pseudo-classes:

-   `:active`: selects an element when it is being activated, such as being clicked
-   `:any-link`: selects an element that acts as a hyperlink
-   `:checked`: selects a form control that is in a checked state (e.g. checkbox or radio)
-   `:default`: selects a form control that is the default value (e.g. submit button)
-   `:dir(ltr/rtl)`: selects an element based on its text direction (left-to-right or right-to-left)
-   `:disabled`: selects a form control that is disabled
-   `:empty`: selects an element that has no children
-   `:enabled`: selects a form control that is enabled
-   `:first-child`: selects an element that is the first child of its parent
-   `:first-of-type`: selects the first element of its type within its parent
-   `:fullscreen`: selects an element that is in full-screen mode
-   `:focus`: selects an element when it has focus, such as when it is selected for input
-   `:focus-within`: selects an element if it or any of its descendants has focus
-   `:hover`: selects an element when the user hovers over it
-   `:indeterminate`: selects a form control that is in an indeterminate state (e.g. progress bar)
-   `:in-range`: selects a form control that has a value within a specified range
-   `:invalid`: selects a form control that is invalid
-   `:lang(language)`: selects an element that is in a specific language
-   `:last-child`: selects an element that is the last child of its parent
-   `:last-of-type`: selects the last element of its type within its parent
-   `:not(selector)`: selects elements that do not match the specified selector
-   `:nth-child(n)`: selects an element that is the nth child of its parent
-   `:nth-last-child(n)`: selects an element that is the nth child of its parent counting from the last child
-   `:nth-last-of-type(n)`: selects the nth element of its type within its parent counting from the last child
-   `:nth-of-type(n)`: selects the nth element of its type within its parent
-   `:only-child`: selects an element that is the only child of its parent
-   `:only-of-type`: selects an element that is the only element of its type within its parent
-   `:optional`: selects a form control that is not required
-   `:out-of-range`: selects a form control that has a value outside of a specified range
-   `:placeholder-shown`: selects a form control that is showing placeholder text
-   `:read-only`: selects a form control that is read-only
-   `:read-write`: selects a form control that is not read-only
-   `:required`: selects a form control that is required
-   `:root`: selects the root element of the document (i.e. `<html>`)
-   `:target`: selects an element that is the target of a fragment identifier in the URL
-   `:valid`: selects a form control that is valid
-   `:visited`: selects a hyperlink that has been visited

Remember that CSS pseudo-classes should be used in combination with other selectors to effectively target elements. They can be used in the following manner:
```css
selector:pseudo-class {
  property: value;
}
```
for example
```css
a:hover {
  color: blue;
}
```
This will change the color of a hyperlink to blue when the user hovers over it.

## CSS pseudo-classes `:is()`, `:where()`, and `:has()`

CSS pseudo-classes `:is()`, `:where()`, and `:has()` are new pseudo-classes in CSS4 and are not yet widely supported by all browsers.

`:is()`: allows for multiple pseudo-classes to be grouped together in a single selector. It takes a list of selectors as its argument and matches elements that match any of the selectors in the list.
```css
:is(selector1, selector2, selector3) {
  property: value;
}
```

`:where()`: is similar to `:is()` but allows for conditions to be specified for the elements being selected. It takes a list of conditions and matches elements that match any of the conditions in the list.
```css
:where(condition1, condition2, condition3) {
  property: value;
}
```

`:has()`: selects elements that have a specified element or pseudo-element as a descendant. It takes a selector as its argument and matches elements that have a descendant matching the selector.
```css
:has(selector) {
  property: value;
}
```
It is important to note that these pseudo-classes are not yet widely supported and may have limited cross-browser compatibility. Before using these pseudo-classes, it is recommended to check browser compatibility and consider alternative solutions if needed.