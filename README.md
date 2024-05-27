
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

