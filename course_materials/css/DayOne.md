# Introduction to CSS

So far you have seen how to use HTML to add content to your webpage. Unfortunately, the content you have created don't look as beautiful or as well laid out as you would want. That is where CSS comes in. You can control the appearance of your page if you know CSS.

Just like a makeup artist, if you are knowledgeable in CSS, you can turn any ugly looking webpage into a beautiful page.

#### What is CSS?

CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of a document written in HTML. It allows you to control the layout, color, font, and overall appearance of your website.

CSS code is just a set of rules that makes declarations as to how the HTML elements should look like or behave.

You write CSS code by first selecting the specific HTML element you want to style and then make the declarations that it should obey.

For example, if you want to style a heading one, you will write H1 (remember you don't need to use the angular brackets '<>') and follow that with a curly bracket. All the declarations that this heading one must obey will be within the curly bracket.

The declarations are written in the form of `name: value`. You can have as many of such declarations as you want. You end each declaration with a semi-colon.

So, to write an example of a CSS rule to turn the heading one into red color, you will write it like this:

```
h1 {
    color: red
}
```

There are a few terminologies that you need to be aware of.

- Selector: In the example above, H1 is referred to as the Selector. That is the part of the CSS code that enables you to select an HTML element. There are different types of selectors and you will learn about them soon.

- Declaration: The part of the CSS code that states both the property and its value. Eg: `color: red;`.

- Declaration block: A group of declarations inside curly braces.

- Ruleset: The selector together with the declaration block are called a ruleset.

![Alt text](image.png)

Now you are aware of what CSS code looks like, let's proceed to learn how you can integrate CSS code into your HTML document.

# Including CSS code in HTML documents
In the previous lesson, you learned the basics of CSS and how it can transform the appearance of your webpages. Now, let's dive into the practical aspect of including CSS code in your HTML documents.

#### Linking External CSS Files

One common way to add CSS to your HTML documents is by linking external CSS files. This approach keeps your HTML code clean and separates the styling from the structure.

To link an external CSS file, you use the `<link>` element within the `<head>` section of your HTML document. Here's an example:

```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <!-- Your HTML content goes here -->
</body>
</html>
```

In this example, we use the `<link>` element's `href` attribute to specify the path to the external CSS file (in this case, "styles.css"). Any styles defined in "styles.css" will be applied to the HTML content.

#### Internal CSS Styles

Alternatively, you can include CSS styles directly within the `<style>` element in the `<head>` section of your HTML document. This approach is useful for adding styles specific to a single webpage.

Here's an example of internal CSS styles:

```html
<!DOCTYPE html>
<html>
<head>
    <style>
        /* CSS styles go here */
        h1 {
            color: blue;
        }
        p {
            font-size: 16px;
        }
    </style>
</head>
<body>
    <!-- Your HTML content goes here -->
</body>
</html>
```

In this example, we define CSS styles directly within the `<style>` element. Any HTML elements matching the selectors will be styled accordingly.

#### Inline CSS Styles

For very specific styles applied to individual HTML elements, you can use inline CSS styles. Inline styles are added directly to an element's `style` attribute.

Here's an example of inline CSS:

```html
<!DOCTYPE html>
<html>
<head>
    <!-- No external or internal CSS -->
</head>
<body>
    <h1 style="color: green;">This is a green heading</h1>
    <p style="font-size: 18px;">This is a larger text.</p>
</body>
</html>
```

In this example, each HTML element has its own inline CSS style defined within the `style` attribute. Inline styles are useful for quick, one-off styling.

Now that you know how to include CSS code in your HTML documents, you're ready to start styling your webpages effectively.

# CSS Selectors

Before we dive into styling web elements with CSS, it's essential to understand how CSS selectors work. CSS selectors are patterns that define which HTML elements should be styled. In this lesson, we'll explore various CSS selectors and how to use them effectively.

#### Universal Selector

The universal selector `*` selects all HTML elements on a webpage. It's a powerful but broad selector that applies styles to every element. For example:

```css
* {
    margin: 0;
    padding: 0;
}
```

In this example, we're removing default margins and padding from all elements on the page.

#### Element Selectors

Element selectors target specific HTML elements by their tag names. For instance:

```css
h1 {
    font-size: 24px;
}
```

This rule sets the font size for all `<h1>` headings on the page.

#### Class Selectors

Class selectors begin with a dot `.` and are used to style elements with a specific class attribute. For example:

```css
.button {
    background-color: #007BFF;
    color: white;
}
```

This rule styles all elements with the `class="button"` attribute.

#### ID Selectors

ID selectors begin with a hash `#` and target a single HTML element with a unique ID attribute. For instance:

```css
#header {
    font-weight: bold;
}
```

This rule styles the element with the `id="header"` attribute.

#### Combining Selectors

You can combine multiple selectors to target specific elements more precisely. For example:

```css
.header h1 {
    color: #333;
}
```

This rule selects `<h1>` elements within an element with the class "header."

#### Descendant Selectors

Descendant selectors target elements nested within other elements. For instance:

```css
ul li {
    list-style-type: square;
}
```

This rule styles `<li>` elements that are descendants of a `<ul>` element.

#### Pseudo-Classes

Pseudo-classes allow you to style elements based on their state or position. For example:

```css
a:hover {
    color: #FF5733;
}
```

This rule changes the color of links when they are hovered over.

#### Attribute Selectors

Attribute selectors allow you to style elements based on their attributes. For example:

```css
input[type="text"] {
    border: 1px solid #CCC;
}
```

This rule styles text input elements.

#### Specificity

Understanding selector specificity is crucial when multiple rules target the same element. Specificity determines which styles take precedence.

In this lesson, you've learned the fundamentals of CSS selectors. They are the building blocks for applying styles to HTML elements. In the next lesson, we'll explore the exciting world of colors in CSS.
