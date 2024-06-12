
### HTML Notes

#### Introduction
HTML (HyperText Markup Language) is the standard language for creating webpages. It describes the structure of a webpage using markup. HTML elements are the building blocks of HTML pages, represented by tags.

#### Editors
To write HTML, you can use various text editors such as:
- **Notepad** (Windows)
- **TextEdit** (Mac)
- **Visual Studio Code**
- **Sublime Text**
- **Atom**

#### Elements
HTML elements are defined by a start tag, content, and an end tag. Example:
```html
<p>This is a paragraph.</p>
```

#### Attributes
Attributes provide additional information about HTML elements. They are always included in the opening tag. Example:
```html
<a href="https://www.example.com">Visit Example</a>
```

#### Headings
HTML headings are defined with the `<h1>` to `<h6>` tags, with `<h1>` being the highest level and `<h6>` the lowest. Example:
```html
<h1>This is a heading</h1>
<h2>This is a subheading</h2>
```

#### Paragraphs
Paragraphs are defined with the `<p>` tag. Example:
```html
<p>This is a paragraph.</p>
```

#### Formatting
HTML provides several tags for formatting text:
- **Bold**: `<b>` or `<strong>`
- **Italic**: `<i>` or `<em>`
- **Underline**: `<u>`
- **Line Break**: `<br>`
- **Horizontal Rule**: `<hr>`
Example:
```html
<p>This is <b>bold</b> and this is <i>italic</i> text.</p>
```

#### Comments
Comments in HTML are not displayed in the browser. They are useful for explaining your code. Example:
```html
<!-- This is a comment -->
```

### CSS Notes

#### Introduction
CSS (Cascading Style Sheets) is used to style and layout web pages. It controls the look and feel of multiple web pages all at once.

#### Syntax
CSS rules are made up of selectors and declarations:
```css
selector {
  property: value;
}
```
Example:
```css
p {
  color: red;
  font-size: 16px;
}
```

#### Applying CSS
CSS can be applied in three ways:
1. **Inline CSS**: Uses the `style` attribute inside HTML elements.
   ```html
   <p style="color: red;">This is a paragraph.</p>
   ```
2. **Internal CSS**: Uses a `<style>` tag within the `<head>` section of an HTML document.
   ```html
   <head>
     <style>
       p { color: red; }
     </style>
   </head>
   ```
3. **External CSS**: Links an external CSS file using the `<link>` tag.
   ```html
   <head>
     <link rel="stylesheet" type="text/css" href="styles.css">
   </head>
   ```
### HTML Colors

HTML colors are used to style elements and improve the visual aesthetics of a webpage. Colors in HTML can be specified using different methods:

#### 1. Named Colors
HTML supports 140 named colors. Example:
```html
<p style="color: red;">This is a red paragraph.</p>
```

#### 2. Hexadecimal Colors
Colors can be defined using a hex code, a combination of six characters (digits and letters) representing the red, green, and blue (RGB) components. The format is `#RRGGBB`.
Example:
```html
<p style="color: #FF0000;">This is a red paragraph.</p>
```
Common hex codes:
- Black: `#000000`
- White: `#FFFFFF`
- Red: `#FF0000`
- Green: `#00FF00`
- Blue: `#0000FF`

#### 3. RGB Colors
Colors can also be defined using the `rgb()` function, specifying the red, green, and blue components as values between 0 and 255.
Example:
```html
<p style="color: rgb(255, 0, 0);">This is a red paragraph.</p>
```

#### 4. RGBA Colors
RGBA is similar to RGB but includes an alpha value (a) for opacity, ranging from 0.0 (completely transparent) to 1.0 (completely opaque).
Example:
```html
<p style="color: rgba(255, 0, 0, 0.5);">This is a semi-transparent red paragraph.</p>
```

#### 5. HSL Colors
HSL stands for Hue, Saturation, and Lightness. Hue is a degree on the color wheel (0-360), saturation is a percentage (0-100%), and lightness is a percentage (0-100%).
Example:
```html
<p style="color: hsl(0, 100%, 50%);">This is a red paragraph.</p>
```

#### 6. HSLA Colors
HSLA is similar to HSL but includes an alpha value for opacity.
Example:
```html
<p style="color: hsla(0, 100%, 50%, 0.5);">This is a semi-transparent red paragraph.</p>
```

#### Using Colors in CSS
Colors are commonly used in CSS to style various elements:
```css
body {
  background-color: #FFFFFF; /* White background */
}

h1 {
  color: #0000FF; /* Blue text */
}

p {
  color: rgb(255, 165, 0); /* Orange text */
}
```

#### Example in HTML
Here’s a full example demonstrating different ways to use colors in HTML:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML Colors Example</title>
  <style>
    body {
      background-color: #F0F0F0; /* Light gray background */
    }
    .hex-color {
      color: #FF5733; /* Hexadecimal color */
    }
    .rgb-color {
      color: rgb(0, 128, 0); /* RGB color */
    }
    .rgba-color {
      color: rgba(0, 0, 255, 0.7); /* RGBA color */
    }
    .hsl-color {
      color: hsl(120, 100%, 25%); /* HSL color */
    }
    .hsla-color {
      color: hsla(240, 100%, 50%, 0.5); /* HSLA color */
    }
  </style>
</head>
<body>
  <h1 style="color: red;">This is a red heading using named color.</h1>
  <p class="hex-color">This is a paragraph with hexadecimal color.</p>
  <p class="rgb-color">This is a paragraph with RGB color.</p>
  <p class="rgba-color">This is a paragraph with RGBA color.</p>
  <p class="hsl-color">This is a paragraph with HSL color.</p>
  <p class="hsla-color">This is a paragraph with HSLA color.</p>
</body>
</html>
```

### HTML Links

HTML links are hyperlinks that allow users to navigate from one page to another or to a different part of the same page. They are created using the `<a>` (anchor) tag.

#### Basic Structure
A basic HTML link is defined with the `<a>` tag and the `href` attribute, which specifies the URL of the page the link goes to.

Example:
```html
<a href="https://www.example.com">Visit Example</a>
```
In this example, "Visit Example" is the clickable text that will take the user to "https://www.example.com".

#### Types of Links

1. **Absolute URLs**
   These URLs point to a location on the web, including the protocol (http, https, etc.).
   ```html
   <a href="https://www.example.com">Visit Example</a>
   ```

2. **Relative URLs**
   These URLs point to a location within the same website. They do not include the domain name.
   ```html
   <a href="/about.html">About Us</a>
   ```

3. **Anchor Links**
   These links point to a specific part of the same page. To create an anchor link, use the `id` attribute to define the target, and the `href` attribute to link to that `id`.
   ```html
   <!-- Target -->
   <h2 id="section1">Section 1</h2>
   <p>Content for section 1.</p>

   <!-- Link -->
   <a href="#section1">Go to Section 1</a>
   ```

4. **Email Links**
   These links open the default email client to send an email.
   ```html
   <a href="mailto:someone@example.com">Send Email</a>
   ```

#### Attributes

1. **target**
   Specifies where to open the linked document.
   - `_blank`: Opens the link in a new tab.
   - `_self`: Opens the link in the same frame (default).
   - `_parent`: Opens the link in the parent frame.
   - `_top`: Opens the link in the full body of the window.

   Example:
   ```html
   <a href="https://www.example.com" target="_blank">Visit Example</a>
   ```

2. **title**
   Provides additional information about the link, which appears as a tooltip when the mouse hovers over the link.
   ```html
   <a href="https://www.example.com" title="Visit Example Website">Visit Example</a>
   ```

3. **download**
   When present, indicates that the target will be downloaded when a user clicks on the hyperlink.
   ```html
   <a href="/files/sample.pdf" download>Download Sample PDF</a>
   ```

#### Styling Links

Links can be styled using CSS. Common pseudo-classes for links include:
- `:link` - A link that has not been visited.
- `:visited` - A link that has been visited.
- `:hover` - A link when the mouse pointer is over it.
- `:active` - A link the moment it is clicked.

Example:
```css
a:link {
  color: blue;
}

a:visited {
  color: purple;
}

a:hover {
  color: red;
}

a:active {
  color: orange;
}
```

#### Example in HTML

Here’s a full example demonstrating different types of links and attributes:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML Links Example</title>
  <style>
    a:link {
      color: blue;
    }
    a:visited {
      color: purple;
    }
    a:hover {
      color: red;
    }
    a:active {
      color: orange;
    }
  </style>
</head>
<body>
  <h1>HTML Links Example</h1>
  <p><a href="https://www.example.com" target="_blank" title="Visit Example Website">Visit Example</a></p>
  <p><a href="/about.html">About Us</a></p>
  <p><a href="#section1">Go to Section 1</a></p>
  <p><a href="mailto:someone@example.com">Send Email</a></p>
  <p><a href="/files/sample.pdf" download>Download Sample PDF</a></p>

  <!-- Anchor target -->
  <h2 id="section1">Section 1</h2>
  <p>This is section 1 of the page.</p>
</body>
</html>
```

### HTML Images

HTML images are used to embed pictures into web pages. Images can enhance the visual appeal and convey information more effectively than text alone. The `<img>` tag is used to embed an image in an HTML document.

#### Basic Structure

The `<img>` tag is an empty tag (self-closing) and does not have a closing tag. It contains attributes that define the source, alternative text, and dimensions of the image.

Example:
```html
<img src="image.jpg" alt="Description of image">
```

#### Attributes

1. **src (source)**
   The `src` attribute specifies the path to the image file. It can be a relative URL, an absolute URL, or a data URL.
   ```html
   <img src="https://www.example.com/image.jpg" alt="Example Image">
   <img src="/images/photo.jpg" alt="Photo">
   ```

2. **alt (alternative text)**
   The `alt` attribute provides alternative text for the image if it cannot be displayed. It is also used by screen readers for accessibility.
   ```html
   <img src="image.jpg" alt="Description of the image">
   ```

3. **width and height**
   These attributes define the width and height of the image in pixels. You can also use CSS to control image dimensions.
   ```html
   <img src="image.jpg" alt="Description of image" width="500" height="300">
   ```

4. **title**
   The `title` attribute provides additional information about the image, which appears as a tooltip when the mouse hovers over the image.
   ```html
   <img src="image.jpg" alt="Description of image" title="This is a tooltip">
   ```

5. **loading**
   The `loading` attribute specifies how the browser should load the image (either `eager` or `lazy`).
   ```html
   <img src="image.jpg" alt="Description of image" loading="lazy">
   ```

#### Examples

##### Example 1: Basic Image
```html
<img src="image.jpg" alt="A beautiful scenery">
```

##### Example 2: Image with Dimensions
```html
<img src="image.jpg" alt="A beautiful scenery" width="600" height="400">
```

##### Example 3: Image with Tooltip
```html
<img src="image.jpg" alt="A beautiful scenery" title="Beautiful Scenery">
```

##### Example 4: Responsive Image
Using CSS to make images responsive:
```html
<style>
  .responsive-img {
    width: 100%;
    height: auto;
  }
</style>
<img src="image.jpg" alt="A beautiful scenery" class="responsive-img">
```

##### Example 5: Lazy Loading Image
```html
<img src="image.jpg" alt="A beautiful scenery" loading="lazy">
```

#### Linking Images

You can also make images clickable by placing them inside an anchor (`<a>`) tag:
```html
<a href="https://www.example.com">
  <img src="image.jpg" alt="Clickable image">
</a>
```

#### Image Formats

Common image formats supported by browsers include:
- **JPEG (.jpg, .jpeg)**: Best for photographs and images with many colors.
- **PNG (.png)**: Supports transparency, good for images with text, logos, and graphics.
- **GIF (.gif)**: Supports animation, best for simple graphics and animations.
- **SVG (.svg)**: Vector format, scalable without loss of quality, good for logos and icons.
- **WebP (.webp)**: Modern format providing superior compression, supports both lossy and lossless compression.

#### Example in HTML

Here’s a full example demonstrating different uses of images:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML Images Example</title>
  <style>
    .responsive-img {
      width: 100%;
      height: auto;
    }
  </style>
</head>
<body>
  <h1>HTML Images Example</h1>

  <!-- Basic Image -->
  <p><img src="image.jpg" alt="A beautiful scenery"></p>

  <!-- Image with Dimensions -->
  <p><img src="image.jpg" alt="A beautiful scenery" width="600" height="400"></p>

  <!-- Image with Tooltip -->
  <p><img src="image.jpg" alt="A beautiful scenery" title="Beautiful Scenery"></p>

  <!-- Responsive Image -->
  <p><img src="image.jpg" alt="A beautiful scenery" class="responsive-img"></p>

  <!-- Lazy Loading Image -->
  <p><img src="image.jpg" alt="A beautiful scenery" loading="lazy"></p>

  <!-- Clickable Image -->
  <p>
    <a href="https://www.example.com">
      <img src="image.jpg" alt="Clickable image">
    </a>
  </p>
</body>
</html>
```


### HTML Tables
HTML tables are used to display data in a tabular format using rows and columns. The main elements involved in creating tables are:

- `<table>`: This tag defines the table.
- `<tr>` (table row): This tag defines a row in the table.
- `<th>` (table header): This tag defines a header cell in the table.
- `<td>` (table data): This tag defines a standard cell in the table.

Example:
```html
<table>
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
```

### HTML Lists
HTML provides two types of lists: ordered and unordered.

- Ordered List (`<ol>`): This list is used when the items have a specific order and is usually displayed with numbers.
- Unordered List (`<ul>`): This list is used when the order of items doesn’t matter and is usually displayed with bullet points.
- List Item (`<li>`): This tag is used to define an item in both ordered and unordered lists.

Example:
```html
<!-- Unordered List -->
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<!-- Ordered List -->
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

### Block and Inline Elements
HTML elements are broadly classified into two categories: block-level and inline-level.

- **Block-Level Elements**: These elements take up the full width of their container and start on a new line. Examples include `<div>`, `<p>`, `<h1>` to `<h6>`, `<ul>`, and `<table>`.
- **Inline-Level Elements**: These elements take up only as much width as necessary and do not start on a new line. Examples include `<span>`, `<a>`, `<img>`, `<strong>`, and `<em>`.

### `<div>` Element
The `<div>` element is a block-level container often used to group other elements together to apply styles or to create layout sections. It's very versatile and commonly used in web development.

Example:
```html
<div class="container">
  <h1>Title</h1>
  <p>This is a paragraph inside a div.</p>
</div>
```

### Classes and IDs
Classes and IDs are used to apply CSS styles and JavaScript functionality to HTML elements.

- **Class**: Defined with the `class` attribute, classes are reusable and can be applied to multiple elements. They are denoted by a period `.` in CSS.

Example:
```html
<p class="highlight">This is a highlighted paragraph.</p>
```
CSS:
```css
.highlight {
  background-color: yellow;
}
```

- **ID**: Defined with the `id` attribute, IDs are unique to a single element on a page. They are denoted by a hash `#` in CSS.

Example:
```html
<p id="unique">This is a unique paragraph.</p>
```
CSS:
```css
#unique {
  color: blue;
}
```



### CSS Backgrounds
CSS provides several properties to set the background of an element.

- `background-color`: Sets the background color.
- `background-image`: Sets a background image.
- `background-repeat`: Controls how a background image is repeated.
- `background-position`: Sets the initial position of a background image.
- `background-size`: Specifies the size of the background image.
- `background-attachment`: Determines whether the background image is fixed or scrolls with the page.

Example:
```css
.element {
  background-color: #f0f0f0;
  background-image: url('image.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
```

### CSS Borders
Borders can be used to set the border around an element.

- `border`: A shorthand property to set the width, style, and color of a border.
- `border-width`: Sets the width of the border.
- `border-style`: Sets the style of the border (solid, dashed, dotted, etc.).
- `border-color`: Sets the color of the border.
- `border-radius`: Rounds the corners of an element's border.

Example:
```css
.element {
  border: 2px solid #000;
  border-radius: 10px;
}
```

### CSS Margin
Margins create space around elements, outside of any defined borders.

- `margin`: A shorthand property for setting the margin on all four sides.
- `margin-top`, `margin-right`, `margin-bottom`, `margin-left`: Individual properties for each side.

Example:
```css
.element {
  margin: 20px;
}
```

### CSS Padding
Padding creates space inside an element, between the content and the border.

- `padding`: A shorthand property for setting the padding on all four sides.
- `padding-top`, `padding-right`, `padding-bottom`, `padding-left`: Individual properties for each side.

Example:
```css
.element {
  padding: 15px;
}
```

### CSS Height and Width
These properties set the height and width of an element.

- `height`: Sets the height of an element.
- `width`: Sets the width of an element.

Example:
```css
.element {
  height: 100px;
  width: 200px;
}
```

### CSS Box Model
The box model represents the structure of an HTML element, including content, padding, border, and margin.

- **Content**: The innermost part where text and images appear.
- **Padding**: Space between the content and the border.
- **Border**: A line surrounding the padding (if any) and content.
- **Margin**: Space outside the border.

Example:
```css
.element {
  width: 200px;
  padding: 10px;
  border: 5px solid #000;
  margin: 20px;
}
```
In this example, the total width of the element would be 250px (200px content + 20px padding + 10px border + 20px margin).

### CSS Outline
The outline is similar to the border but does not affect the size of the element or the box model. It's drawn outside the border edge.

- `outline`: A shorthand property for setting the outline width, style, and color.
- `outline-width`: Sets the width of the outline.
- `outline-style`: Sets the style of the outline.
- `outline-color`: Sets the color of the outline.
- `outline-offset`: Specifies the space between the outline and the border edge.

Example:
```css
.element {
  outline: 2px dashed red;
  outline-offset: 5px;
}
```

### CSS Text
CSS provides various properties to style text, including color, alignment, decoration, and transformation.

- `color`: Sets the color of the text.
- `text-align`: Aligns the text (left, right, center, justify).
- `text-decoration`: Adds decoration to text (underline, overline, line-through).
- `text-transform`: Controls the capitalization of text (uppercase, lowercase, capitalize).
- `line-height`: Sets the space between lines of text.
- `text-shadow`: Adds shadow to text.

Example:
```css
.text {
  color: #333;
  text-align: center;
  text-decoration: underline;
  text-transform: uppercase;
  line-height: 1.5;
  text-shadow: 2px 2px #888;
}
```

### CSS Fonts
CSS allows you to specify fonts and their styles.

- `font-family`: Specifies the font family.
- `font-size`: Sets the size of the font.
- `font-weight`: Sets the weight of the font (boldness).
- `font-style`: Sets the style of the font (normal, italic, oblique).
- `font-variant`: Controls the use of small-caps font.

Example:
```css
.text {
  font-family: 'Arial, sans-serif';
  font-size: 16px;
  font-weight: bold;
  font-style: italic;
  font-variant: small-caps;
}
```

### CSS Icons
Icons can be added using icon libraries such as Font Awesome or by using custom images.

- Using Font Awesome:
  ```html
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
  <i class="fas fa-camera"></i>
  ```

- Using custom images:
  ```html
  <img src="icon.png" alt="Icon" class="icon">
  ```
  ```css
  .icon {
    width: 32px;
    height: 32px;
  }
  ```

### CSS Links
Links can be styled using the `a` tag with different states: normal, visited, hover, and active.

- `a`: Normal link state.
- `a:visited`: Visited link state.
- `a:hover`: Link state when hovered over.
- `a:active`: Link state when clicked.

Example:
```css
a {
  color: blue;
  text-decoration: none;
}

a:hover {
  color: darkblue;
  text-decoration: underline;
}

a:visited {
  color: purple;
}

a:active {
  color: red;
}
```

### CSS Lists
Lists can be styled to change their appearance, including removing bullets or numbers, and setting custom styles.

- `list-style-type`: Changes the bullet or numbering style (none, disc, circle, square, decimal, etc.).
- `list-style-image`: Uses an image as the list item marker.
- `list-style-position`: Specifies the position of the list-item markers (inside, outside).

Example:
```css
ul {
  list-style-type: square;
}

ol {
  list-style-type: upper-roman;
}

.custom-list {
  list-style-type: none;
}

.custom-list li {
  background: url('custom-marker.png') no-repeat left center;
  padding-left: 20px;
}
```

### CSS Tables
Tables can be styled to improve their appearance and readability.

- `border-collapse`: Specifies whether table borders should collapse into a single border or be separated.
- `border-spacing`: Sets the distance between the borders of adjacent cells.
- `table-layout`: Specifies the layout algorithm (auto, fixed).
- `width`: Sets the width of the table.
- `text-align`: Aligns text in table cells.
- `vertical-align`: Aligns the content vertically in a table cell.
- `padding`: Adds padding to table cells.
- `background-color`: Sets the background color of table elements.

Example:
```css
table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: left;
}

th {
  background-color: #f2f2f2;
}

tr:nth-child(even) {
  background-color: #f9f9f9;
}

tr:hover {
  background-color: #f1f1f1;
}
```

### Summary
- **Text**: Use properties like color, alignment, decoration, transformation, line-height, and shadow.
- **Fonts**: Specify font family, size, weight, style, and variant.
- **Icons**: Include using icon libraries or custom images.
- **Links**: Style different link states (normal, visited, hover, active).
- **Lists**: Customize list markers and positions.
- **Tables**: Style table borders, spacing, layout, and cell content for better readability.


### CSS Display
The `display` property specifies how an element is displayed on the page.

- `display: block`: The element is displayed as a block-level element (e.g., `<div>`, `<p>`).
- `display: inline`: The element is displayed as an inline element (e.g., `<span>`, `<a>`).
- `display: inline-block`: The element is displayed as an inline element but can have block-level properties (like width and height).
- `display: none`: The element is not displayed at all (it’s removed from the document flow).
- `display: flex`: The element becomes a flex container, and its children are flex items.
- `display: grid`: The element becomes a grid container, and its children are grid items.

Example:
```css
.block {
  display: block;
}

.inline {
  display: inline;
}

.inline-block {
  display: inline-block;
}

.none {
  display: none;
}

.flex {
  display: flex;
}

.grid {
  display: grid;
}
```

### CSS max-width
The `max-width` property sets the maximum width of an element. It prevents the element from becoming wider than the specified value.

Example:
```css
.container {
  max-width: 100%;
}

.content {
  max-width: 800px;
}
```

### CSS Position
The `position` property specifies the type of positioning method used for an element.

- `position: static`: The default positioning; elements are positioned according to the normal flow of the document.
- `position: relative`: The element is positioned relative to its normal position.
- `position: absolute`: The element is positioned relative to the nearest positioned ancestor (not static).
- `position: fixed`: The element is positioned relative to the browser window, and it stays fixed during scrolling.
- `position: sticky`: The element is positioned based on the user's scroll position.

Example:
```css
.static {
  position: static;
}

.relative {
  position: relative;
  top: 10px;
  left: 20px;
}

.absolute {
  position: absolute;
  top: 50px;
  left: 100px;
}

.fixed {
  position: fixed;
  top: 0;
  right: 0;
}

.sticky {
  position: sticky;
  top: 0;
}
```

### CSS z-index
The `z-index` property specifies the stack order of an element. It only works on positioned elements (relative, absolute, fixed, sticky).

- Higher `z-index` values indicate that the element is in front of those with lower values.

Example:
```css
.behind {
  position: relative;
  z-index: 1;
}

.in-front {
  position: relative;
  z-index: 2;
}
```

### CSS Overflow
The `overflow` property specifies what happens if content overflows an element's box.

- `overflow: visible`: The overflow is not clipped. The content renders outside the element’s box.
- `overflow: hidden`: The overflow is clipped, and the rest of the content is invisible.
- `overflow: scroll`: The overflow is clipped, and a scrollbar is added to see the rest of the content.
- `overflow: auto`: Similar to `scroll`, but scrollbars are added only when necessary.

Example:
```css
.visible {
  overflow: visible;
}

.hidden {
  overflow: hidden;
}

.scroll {
  overflow: scroll;
}

.auto {
  overflow: auto;
}
```

### CSS Float
The `float` property is used for positioning and formatting content by allowing elements to float to the left or right of their container.

- `float: left`: Floats the element to the left.
- `float: right`: Floats the element to the right.
- `float: none`: The element does not float.

To clear floated elements, use the `clear` property.

Example:
```css
.left {
  float: left;
}

.right {
  float: right;
}

.none {
  float: none;
}

.clearfix::after {
  content: "";
  display: table;
  clear: both;
}
```

### Summary
- **Display**: Controls how an element is displayed (`block`, `inline`, `none`, `flex`, `grid`).
- **max-width**: Sets the maximum width of an element.
- **Position**: Controls the positioning method of an element (`static`, `relative`, `absolute`, `fixed`, `sticky`).
- **z-index**: Controls the stack order of positioned elements.
- **Overflow**: Specifies what happens when content overflows an element’s box (`visible`, `hidden`, `scroll`, `auto`).
- **Float**: Allows elements to float to the left or right of their container and uses the `clear` property to manage float behavior.


### CSS Flexbox

Flexbox (Flexible Box Layout) is a CSS layout module designed to arrange and align items within a container efficiently. Flexbox makes it easier to design flexible and responsive layouts, allowing elements to adapt to different screen sizes and display devices.

### Key Concepts

#### 1. **Flex Container and Flex Items**
- **Flex Container**: An element with `display: flex` or `display: inline-flex`.
- **Flex Items**: The direct children of a flex container.

```css
.container {
    display: flex; /* or inline-flex */
}
```

### Flex Container Properties

#### 2. **flex-direction**
Defines the direction in which the flex items are placed in the flex container.

- `row`: Default value. Items are placed in a row (left to right in ltr; right to left in rtl).
- `row-reverse`: Items are placed in a row in reverse order (right to left in ltr; left to right in rtl).
- `column`: Items are placed in a column (top to bottom).
- `column-reverse`: Items are placed in a column in reverse order (bottom to top).

```css
.container {
    flex-direction: row; /* row | row-reverse | column | column-reverse */
}
```

#### 3. **flex-wrap**
Specifies whether the flex items should wrap or not when there is not enough space.

- `nowrap`: Default value. Items are placed in a single line.
- `wrap`: Items wrap onto multiple lines.
- `wrap-reverse`: Items wrap onto multiple lines in reverse order.

```css
.container {
    flex-wrap: wrap; /* nowrap | wrap | wrap-reverse */
}
```

#### 4. **flex-flow**
A shorthand for `flex-direction` and `flex-wrap`.

```css
.container {
    flex-flow: row wrap; /* <'flex-direction'> <'flex-wrap'> */
}
```

#### 5. **justify-content**
Aligns flex items along the main axis (horizontally if `flex-direction` is `row`).

- `flex-start`: Default value. Items are aligned to the start of the container.
- `flex-end`: Items are aligned to the end of the container.
- `center`: Items are centered in the container.
- `space-between`: Items are evenly distributed; the first item is at the start, the last item is at the end.
- `space-around`: Items are evenly distributed with space around them.
- `space-evenly`: Items are evenly distributed with equal space between them.

```css
.container {
    justify-content: center; /* flex-start | flex-end | center | space-between | space-around | space-evenly */
}
```

#### 6. **align-items**
Aligns flex items along the cross axis (vertically if `flex-direction` is `row`).

- `stretch`: Default value. Items are stretched to fill the container.
- `flex-start`: Items are aligned to the start of the cross axis.
- `flex-end`: Items are aligned to the end of the cross axis.
- `center`: Items are centered along the cross axis.
- `baseline`: Items are aligned along their baselines.

```css
.container {
    align-items: center; /* stretch | flex-start | flex-end | center | baseline */
}
```

#### 7. **align-content**
Aligns flex lines within the flex container when there is extra space along the cross axis.

- `stretch`: Default value. Lines stretch to take up the remaining space.
- `flex-start`: Lines are packed to the start of the container.
- `flex-end`: Lines are packed to the end of the container.
- `center`: Lines are centered in the container.
- `space-between`: Lines are evenly distributed with the first line at the start and the last line at the end.
- `space-around`: Lines are evenly distributed with space around them.
- `space-evenly`: Lines are evenly distributed with equal space between them.

```css
.container {
    align-content: space-around; /* stretch | flex-start | flex-end | center | space-between | space-around | space-evenly */
}
```

### Flex Item Properties

#### 8. **order**
Specifies the order of a flex item relative to the other flex items. Default is 0.

```css
.item {
    order: 1; /* default is 0 */
}
```

#### 9. **flex-grow**
Specifies how much a flex item will grow relative to the other flex items when there is extra space in the flex container. Default is 0.

```css
.item {
    flex-grow: 2; /* default is 0 */
}
```

#### 10. **flex-shrink**
Specifies how much a flex item will shrink relative to the other flex items when there is not enough space in the flex container. Default is 1.

```css
.item {
    flex-shrink: 1; /* default is 1 */
}
```

#### 11. **flex-basis**
Specifies the initial size of a flex item before any space distribution. It can be a length (px, em, etc.) or a percentage.

```css
.item {
    flex-basis: 100px; /* default is auto */
}
```

#### 12. **flex**
A shorthand for `flex-grow`, `flex-shrink`, and `flex-basis`.

```css
.item {
    flex: 1 1 100px; /* <flex-grow> <flex-shrink> <flex-basis> */
}
```

#### 13. **align-self**
Overrides the `align-items` property for a specific flex item, allowing for individual alignment.

- `auto`: Default. Inherits the value from the `align-items` property of the flex container.
- `flex-start`: Aligns the item to the start of the cross axis.
- `flex-end`: Aligns the item to the end of the cross axis.
- `center`: Centers the item along the cross axis.
- `baseline`: Aligns the item along its baseline.
- `stretch`: Stretches the item to fill the container.

```css
.item {
    align-self: flex-end; /* auto | flex-start | flex-end | center | baseline | stretch */
}
```

### Example

Here is an example that demonstrates various flexbox properties:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Example</title>
    <style>
        .container {
            display: flex;
            flex-direction: row;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            height: 200px;
            border: 1px solid #ccc;
        }
        .item {
            background-color: #4CAF50;
            color: white;
            padding: 10px;
            margin: 5px;
            flex: 1;
            text-align: center;
        }
        .item:nth-child(2) {
            flex-grow: 2;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
    </div>
</body>
</html>
```



