- [[#HTML Document Structure]]
- [[#Basic HTML Elements]]
- [[#HTML Tables]]
- [[#HTML Forms]]
	- [[#Input Elements]]
	- [[#Textareas]]
	- [[#Select Elements]]
	- [[#Form Attributes]]
- [[#HTML Semantic Elements]]
- [[#HTML Attributes]]
- [[#HTML Entities]]
- [[#HTML Charset]]
- [[#HTML Styles]]
- [[#HTML Media]]
	- [[#Images]]
	- [[#Videos]]
	- [[#Audio]]
- [[#ARIA (Accessible Rich Internet Applications)]]



## HTML Document Structure
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Document Title</title>
  </head>
  <body>
    <!-- Content Goes Here -->
  </body>
</html>
```

## Basic HTML Elements
```html
<!-- Heading -->
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>

<!-- Paragraph -->
<p>This is a paragraph.</p>

<!-- Link -->
<a href="https://www.example.com">Example Link</a>

<!-- Image -->
<img src="image.jpg" alt="Image Description">

<!-- List -->
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

## HTML Tables

Tables are used to display tabular data. A table is created using the `<table>` element, and rows are added using the `<tr>` element. Table cells are added using the `<td>` element, and table headers are added using the `<th>` element.
```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Row 1, Column 1</td>
    <td>Row 1, Column 2</td>
  </tr>
  <tr>
    <td>Row 2, Column 1</td>
    <td>Row 2, Column 2</td>
  </tr>
</table>

```


## HTML Forms
HTML forms allow you to collect data from users. A form is created using the `<form>` element, and form controls, such as text fields, checkboxes, and buttons, are added using various other HTML elements.

### Input Elements

-   `<input type="text">`: text input field
-   `<input type="password">`: password input field
-   `<input type="radio">`: radio button
-   `<input type="checkbox">`: checkbox
-   `<input type="submit">`: submit button
-   `<input type="reset">`: reset button

### Textareas
-   `<textarea>`: multi-line text input field

### Select Elements
-   `<select>`: drop-down list
-   `<option>`: list item in a drop-down list

### Form Attributes
-   `action`: the URL to submit the form data to
-   `method`: the HTTP method to use for submitting the form data (`GET` or `POST`)
-   `enctype`: the encoding type of the form data (`application/x-www-form-urlencoded` or `multipart/form-data`)

```html
<!-- Form -->
<form action="https://www.example.com" method="post">
  <!-- Input -->
  <label for="input">Input Label:</label>
  <input type="text" id="input" name="input">
  
  <!-- Select -->
  <label for="select">Select Label:</label>
  <select id="select" name="select">
    <option value="option1">Option 1</option>
    <option value="option2">Option 2</option>
    <option value="option3">Option 3</option>
  </select>
  
  <!-- Checkbox -->
  <input type="checkbox" id="checkbox" name="checkbox">
  <label for="checkbox">Checkbox Label</label>
  
  <!-- Radio -->
  <input type="radio" id="radio1" name="radio" value="radio1">
  <label for="radio1">Radio 1</label>
  <input type="radio" id="radio2" name="radio" value="radio2">
  <label for="radio2">Radio 2</label>
  
  <!-- Submit -->
  <input type="submit" value="Submit">
</form>
```

## HTML Semantic Elements
```html
<header>Header</header>
<nav>Navigation</nav>
<main>Main Content</main>
<aside>Aside</aside>
<footer>Footer</footer>
<article>Article</article>
<section>Section</section>
```

## HTML Attributes

Some common HTML attributes include:

-   `class`: used to apply CSS styles
-   `id`: used to uniquely identify an element
-   `src`: used to specify the source of an element, such as an image file
-   `href`: used to specify the URL of a linked resource
-   `alt`: used to provide a text description of an image
-   `width` and `height`: used to specify the dimensions of an element
-   `style`: used to apply inline CSS styles
-   `target`: used to specify where a linked resource should open
-   `colspan` and `rowspan`: used to specify the number of columns or rows a table cell should span
-   `disabled`: used to disable a form element
-   `value`: used to specify the value of a form element

## HTML Entities

Some common HTML entities include:

-   `&lt;`: less than symbol (<)
-   `&gt;`: greater than symbol (>)
-   `&amp;`: ampersand (&)
-   `&quot;`: quotation mark (")
-   `&copy;`: copyright symbol (©)
-   `&reg;`: registered trademark symbol (®)

## HTML Charset

To specify the character encoding of an HTML document, use the `<meta>` element with the `charset` attribute:
```html
<meta charset="UTF-8">
```

## HTML Styles

To add styles to an HTML document, you can use three methods:

1.  Inline styles using the `style` attribute on an HTML element
```html
<p style="color: red;">This is a red paragraph.</p>
```

2.  Internal styles using a `<style>` element in the `<head>` of the HTML document
```html
<head>
	<style>
		p { color: red; } 
	</style>
</head>
```

3.  External styles using a separate CSS file linked to the HTML document using a `<link>` element in the `<head>` of the HTML document
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

## HTML Media

HTML supports various types of media, such as images, videos, and audio.

### Images

To add an image to an HTML document, use the `<img>` element with the `src` attribute to specify the source of the image and the `alt` attribute to provide a text description:
```html
<img src="image.jpg" alt="An example image">
```

### Videos

To add a video to an HTML document, use the `<video>` element with the `src` attribute to specify the source of the video and the `controls` attribute to show the video controls:
```html
<video src="video.mp4" controls></video>
```

### Audio

To add audio to an HTML document, use the `<audio>` element with the `src` attribute to specify the source of the audio and the `controls` attribute to show the audio controls:
```html
<audio src="audio.mp3" controls></audio>
```

## ARIA (Accessible Rich Internet Applications)

ARIA is a system for adding additional semantic information to HTML elements, making it easier for assistive technologies, such as screen readers, to understand the meaning and structure of a web page.

### ARIA Roles

ARIA roles describe the purpose of an element, such as a button, a checkbox, or a navigation menu. Some common ARIA roles include:

-   `role="button"`: indicates that an element should be treated as a button
-   `role="checkbox"`: indicates that an element should be treated as a checkbox
-   `role="navigation"`: indicates that an element contains navigation links
-   `role="menuitem"`: indicates that an element is a menu item
-   `role="tab"`: indicates that an element should be treated as a tab in a tab panel

### ARIA Attributes

ARIA attributes provide additional information about an element, such as the state of a checkbox or the current tab in a tab panel. Some common ARIA attributes include:

-   `aria-checked`: indicates the state of a checkbox or toggle button (`true` or `false`)
-   `aria-selected`: indicates the selected state of an element, such as a tab in a tab panel (`true` or `false`)
-   `aria-hidden`: indicates whether an element is hidden or visible (`true` or `false`)
-   `aria-expanded`: indicates whether an element, such as a dropdown menu, is expanded or collapsed (`true` or `false`)
-   `aria-labelledby`: associates an element with a label, specified by the value of this attribute (the ID of the label element)
-   `aria-describedby`: associates an element with a description, specified by the value of this attribute (the ID of the description element)

### ARIA Live Regions

ARIA live regions allow you to update parts of a web page dynamically, without causing the entire page to refresh. When the content of a live region changes, assistive technologies, such as screen readers, will announce the changes to users. To create a live region, you can use the `role` attribute and the `aria-live` attribute:
```html
<div role="status" aria-live="polite">
  This is a live region. The content of this region will be updated dynamically.
</div>
```

The value of the `aria-live` attribute determines the priority of the updates:

-   `polite`: updates should be announced when the user is idle
-   `assertive`: updates should be announced immediately

### ARIA Implementation Best Practices

-   Use native HTML elements whenever possible, and only use ARIA roles, attributes, and live regions as a fallback when native HTML elements do not provide the necessary semantics.
-   Test your implementation with assistive technologies, such as screen readers, to ensure that it is accessible to users with disabilities.
-   Follow the ARIA specification, as well as any guidance provided by the Web Content Accessibility Guidelines (WCAG), to ensure that your implementation is accessible and usable.

## Additional ARIA Roles

Here are some more ARIA roles:

-   `role="application"`: indicates that an element should be treated as an application
-   `role="banner"`: indicates that an element contains the site or application's banner content
-   `role="complementary"`: indicates that an element contains content that complements the main content, but can still be understood on its own
-   `role="contentinfo"`: indicates that an element contains information about the parent document or application
-   `role="dialog"`: indicates that an element should be treated as a dialog or alert dialog
-   `role="main"`: indicates that an element contains the main content of the document

## Additional ARIA Attributes

Here are some more ARIA attributes:

-   `aria-activedescendant`: identifies the currently active descendant of a widget, such as a listbox or tree
-   `aria-atomic`: indicates whether an element's changes should be announced to assistive technologies as a single unit, or one change at a time
-   `aria-controls`: associates an element with the elements it controls, specified by the value of this attribute (a space-separated list of the IDs of the controlled elements)
-   `aria-flowto`: associates an element with elements that it flows to, specified by the value of this attribute (a space-separated list of the IDs of the elements that it flows to)
-   `aria-labelledby`: associates an element with a label, specified by the value of this attribute (the ID of the label element)
-   `aria-level`: indicates the level of an element within a structure, such as a heading or list item
-   `aria-multiselectable`: indicates whether a user can select more than one item in a widget, such as a listbox or grid
-   `aria-orientation`: indicates the orientation of a widget, such as a scrollbar or slider
-   `aria-owns`: associates an element with the elements it controls, specified by the value of this attribute (a space-separated list of the IDs of the controlled elements)

## ARIA in Practice

Using ARIA roles and attributes effectively requires a solid understanding of accessibility and HTML, as well as a good understanding of the ARIA specification. Some tips for using ARIA in practice include:

-   Use roles and attributes consistently and correctly
-   Provide alternative text for images and other non-text content, as needed
-   Use ARIA live regions to update content dynamically, but do so in a way that does not interfere with the user's ability to interact with the page
-   Test your implementation with assistive technologies, such as screen readers, to ensure that it is accessible to users with disabilities.

## ARIA and JavaScript

When using JavaScript to manipulate the content of a page, it's important to also update the ARIA attributes and roles as needed, to ensure that the changes are communicated to assistive technologies. For example:

-   When expanding or collapsing content, use JavaScript to update the `aria-expanded` attribute accordingly
-   When changing the focus of a widget, use JavaScript to update the `aria-activedescendant` attribute
-   When adding or removing items from a list, use JavaScript to update the `aria-level`, `aria-setsize`, and `aria-posinset` attributes, if applicable

## Conclusion

The ARIA semantic system is a powerful tool for improving the accessibility of web content, but it requires a good understanding of accessibility and HTML, as well as a solid understanding of the ARIA specification. When used effectively, ARIA can help make your content more accessible to users with disabilities, and ensure that assistive technologies provide a usable and accessible experience.

