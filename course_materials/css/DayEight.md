# Text Styling in CSS
Text is a fundamental component of web content, and CSS provides extensive tools for styling and formatting text to create visually appealing webpages. In this lesson, we'll explore various CSS properties to style and enhance text.

#### Text Color

The `color` property allows you to define the color of text. You can use named colors, hexadecimal values, RGB values, or HSL values. For example:

```css
p {
    color: #333; /* Dark gray text */
}
```

This rule sets the color of all paragraphs to dark gray.

#### Text Alignment

The `text-align` property controls the horizontal alignment of text within an element. It can be set to values like `left`, `right`, `center`, or `justify`. For example:

```css
h1 {
    text-align: center;
}
```

This rule centers the text within `<h1>` headings.

#### Text Decoration

In addition to underlines and overlines, you can use the `text-decoration` property to apply a line-through or blink effect to text. For example:

```css
del {
    text-decoration: line-through;
}
```

This rule adds a line-through effect to text within `<del>` elements.

#### Letter Spacing and Word Spacing

The `letter-spacing` property adjusts the spacing between characters, while the `word-spacing` property controls spacing between words. For example:

```css
blockquote {
    letter-spacing: 2px;
    word-spacing: 5px;
}
```

This rule increases the spacing between characters and words within `<blockquote>` elements.

#### Text Transformation

CSS offers text transformation properties like `text-transform` to change the capitalization of text. Values include `uppercase`, `lowercase`, and `capitalize`. For example:

```css
button {
    text-transform: uppercase;
}
```

This rule transforms the text within `<button>` elements to uppercase.

#### Line Height

The `line-height` property adjusts the vertical spacing between lines of text. It can be set as a numeric value, percentage, or unit. For example:

```css
p {
    line-height: 1.5; /* 150% line height */
}
```

This rule increases the line height for all paragraphs.

#### Text Shadow

You can create text shadow effects using the `text-shadow` property, which allows you to specify the color, horizontal offset, vertical offset, and blur radius of the shadow. For example:

```css
h2 {
    text-shadow: 2px 2px 4px #333; /* Gray shadow */
}
```

This rule adds a gray shadow to text within `<h2>` headings.

#### Font Family and Size

In combination with the previous lessons on fonts, you can further style text by specifying font families and sizes to create unique text presentations.

In this lesson, you've explored various CSS properties to style text, from color and alignment to decoration and transformation. Effective text styling can greatly enhance the readability and visual appeal of your webpages.

# Measurement Units in CSS
In CSS, you have the flexibility to control the size and dimensions of elements using different measurement units. Understanding these units and when to use them is crucial for creating responsive and visually appealing web designs. In this lesson, we'll explore the common measurement units in CSS.

#### Pixels (px)

Pixels, denoted as `px`, are the most commonly used measurement unit in CSS. They provide a fixed size relative to the screen's pixel density. For example:

```css
h1 {
    font-size: 24px;
    width: 300px;
    height: 150px;
}
```

In this rule, the `<h1>` heading has a font size of 24 pixels, and its width and height are set to fixed pixel values.

#### Percentages (%)

Percentage units represent a portion of the parent element's size. They are particularly useful for creating responsive designs. For example:

```css
.container {
    width: 80%;
    padding: 5%;
}
```

In this rule, the `.container` element's width and padding are specified as percentages of its parent's width.

#### em and rem

The `em` unit represents the font size of the current element. `rem` (root em) is similar but based on the root element's font size. These units are useful for maintaining relative proportions. For example:

```css
p {
    font-size: 1.2em;
}
```

This rule sets the font size of paragraphs to 1.2 times their parent element's font size.

#### Viewport Units (vw, vh, vmin, vmax)

Viewport units are relative to the viewport's dimensions (the visible area of the browser window). They allow you to create designs that adapt to the screen size. For example:

```css
header {
    width: 80vw; /* 80% of viewport width */
    height: 50vh; /* 50% of viewport height */
}
```

In this rule, the `header` element's width and height are set as percentages of the viewport's dimensions.

#### Absolute Units (in, cm, mm, pt, pc)

Absolute units provide fixed measurements and are less commonly used in web design due to their lack of responsiveness. For example:

```css
table {
    width: 8in; /* 8 inches */
    height: 10cm; /* 10 centimeters */
}
```

These units specify fixed dimensions for a `<table>` element.

#### Ch and Rem Units for Text

The `ch` unit represents the width of the character '0' in the current font, while `rem` is based on the root font size. These units are valuable for sizing text elements. For example:

```css
code {
    font-size: 0.8rem;
    width: 20ch;
}
```

In this rule, the `code` element's font size is relative to the root font size, and its width is based on the width of 20 '0' characters.

Understanding the various measurement units in CSS allows you to create responsive and adaptable web designs. Choosing the appropriate unit for each context is essential for achieving your desired layout and styling.

# Working with Images in CSS
Images are essential components of web design, and CSS provides tools to style and manipulate them to enhance the visual appeal of your webpages. In this lesson, we'll explore how to work with images in CSS.

#### Adding Images

To add an image to your webpage, you can use the `background-image` property. For example:

```css
.header {
    background-image: url('header-image.jpg');
    background-size: cover;
    height: 300px;
}
```

In this rule, the `.header` element sets a background image from 'header-image.jpg' and adjusts its size to cover the entire element.

#### Background Properties

CSS offers various background properties to control the display and positioning of background images:

- `background-repeat`: Specifies whether the background image should repeat, no-repeat, repeat-x, or repeat-y.

- `background-position`: Determines the position of the background image within its container.

- `background-attachment`: Sets whether the background image scrolls with the content or remains fixed.

#### Image Opacity

You can control the opacity of an image using the `opacity` property. For example:

```css
.img-container {
    opacity: 0.7; /* 70% opacity */
}
```

This rule makes the content of the `.img-container` element 70% transparent.

#### Image Filters

CSS allows you to apply various filters to images using the `filter` property. You can adjust properties like `brightness`, `contrast`, `grayscale`, `blur`, and more to create unique visual effects. For example:

```css
.img-filter {
    filter: grayscale(50%) blur(3px);
}
```

This rule applies a 50% grayscale filter and a 3-pixel blur effect to the `.img-filter` element.

#### Image as Content

You can also use the `content` property to insert images as content within HTML elements. For example:

```css
blockquote::before {
    content: url('quote-icon.png');
    margin-right: 5px;
}
```

This rule adds a quote icon before every `<blockquote>` element.

#### Responsive Images

To make images responsive and adapt to different screen sizes, use the `max-width` property. For example:

```css
img {
    max-width: 100%;
    height: auto;
}
```

This rule ensures that images never exceed their parent container's width and maintain their aspect ratio.

#### Image Sprites

Image sprites involve combining multiple images into a single file and using CSS to display specific parts of the image as needed. This technique reduces the number of server requests and improves loading times.

Understanding how to work with images in CSS allows you to create visually engaging webpages.
