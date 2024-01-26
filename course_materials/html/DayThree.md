# Attributes
Attributes in HTML provide additional information about elements, usually in the form of name-value pairs, and are placed within the element's opening tag. Attributes are used to modify the default functionality of an element or to provide metadata. They can control a wide range of behaviors and properties.

Here are a few key points about attributes:

Structure: Attributes are defined within the opening tag of an element and consist of a name followed by an equal sign and a value. The value should be enclosed in quotes. For example: `<div id="header">`.

You will commonly use attributes when working with links and images which you will be looking at after this lesson.

Some other common uses include using attributes like class and id to mark elements for styling or manipulation with JavaScript. You can also directly add CSS styles to an HTML element by using the `style` attribute.

eg: `<span style="color:red">`

#### Must know
**Boolean Attributes**: Some attributes don't require a value and are either present or not. For example, the disabled attribute can be added to a button to make it non-interactive: <button disabled>Click Me!</button>.

**Global Attributes**: These are attributes that can be used with any element. Examples include id, class, style, and title.

**Importance of Correct Usage**: Using attributes correctly is crucial for accessibility, usability, and maintaining valid code. For instance, the alt attribute on images is a vital consideration for users who rely on screen readers.

As you work with different elements, becoming familiar with their specific attributes and values is key to effective web development.

# Links and Images
Links and Images are essential components of almost every webpage.

## Links (Anchors) in HTML
Links, created with the `<a>`` (anchor) element, are one of the fundamental components of the web, allowing users to navigate from one resource to another with a click. Here are some key points about HTML links:

1. Syntax: The basic syntax for a link is `<a href="URL">link text</a>`, where href is the attribute that specifies the destination of the link, and "link text" is the clickable text in the document.

2. Attributes:
    - href (Hypertext REFerence): Specifies the URL of the page the link goes to.
    - target: Defines where the linked document will open, such as _blank for a new tab.
    - title: Provides additional information about the link, usually displayed as a tooltip.

3. Types of Links:
    - External Links: Link to a different website.
    - Internal Links: Navigate within the same website or document.
    - Anchor Links: Jump to a specific part of a webpage using an element's ID.


## Images in HTML
Images are added to HTML documents using the <img> tag and are crucial for adding visual elements to web pages. Here are some key points about HTML images:

1. Syntax: The basic syntax for an image is `<img src="URL" alt="description">`.

2. Attributes:
    - src (Source): Specifies the path to the image.
    - alt (Alternative Text): Provides a text alternative for the image. This is crucial for accessibility, as screen readers read this text aloud to describe the image to users who can't see it.
    - width and height: Define the size of the image.
    - title: Offers additional information about the image, usually displayed as a tooltip.

3. Formats: Common image formats used on the web include JPEG, PNG, GIF, and with increasing support, WebP and SVG. Each format has its own use case and trade-offs between quality and file size.


When using links and images, remember to provide fallbacks or alternative content to ensure a good user experience and accessibility. For instance, always include the alt attribute for images, and ensure your link text is descriptive enough to make sense out of context. These elements, when used effectively, enhance the navigability and visual appeal of websites.


### Task: Create a Personal Webpage with Links and Images

In this exercise, you'll create a simple personal webpage. This page will include headings, paragraphs, an image of yourself or a favorite item, and links to your favorite websites. Through this task, you'll practice using various HTML elements and understand the importance of each.

#### Step 1: Set Up Basic HTML Structure

- **Task**: Start by setting up the basic structure of an HTML document. Create a new folder/directory and call it `personal-website`
- **Code**:
  ```html
  <!DOCTYPE html>
  <html>
  <head>
    <title>My Personal Webpage</title>
  </head>
  <body>
  
  </body>
  </html>
  ```
- **Essence**: The `<!DOCTYPE html>` declaration defines the document to be HTML5. The `<html>` element is the root element of an HTML page. The `<head>` section is where you include meta information and the `<title>` tag is for the title of the document that shows up in the browser tab. The `<body>` is where all visible content goes.

#### Step 2: Add Headings and Paragraphs

- **Task**: Introduce yourself using headings and a brief paragraph.
- **Code**:
  ```html
  <h1>Welcome to My Personal Webpage</h1>
  <h2>About Me</h2>
  <p>Hello! My name is [Your Name]. I'm learning HTML from LearninBits to create amazing websites!</p>
  ```
- **Essence**: `<h1>` and `<h2>` are heading elements that organize and provide structure to your webpage. They are important for readability and SEO. `<p>` represents a paragraph of text, providing a way to group related content.

#### Step 3: Insert an Image

- **Task**: Add an image to represent yourself or something you like.
- **Code**:
  ```html
  <img src="path_to_image.jpg" alt="Description of image">
  ```
- **Essence**: The `<img>` tag embeds an image in the HTML page. `src` attribute specifies the path to the image, and `alt` provides alternative text which is crucial for accessibility and in cases where the image cannot be displayed.

#### Step 4: Add Links to Favorite Websites

- **Task**: Create a list of your favorite websites with links.
- **Code**:
  ```html
  <h2>My Favorite Websites</h2>
  <p><a href="https://www.example.com" target="_blank">Example Site 1</a></p>
  <p><a href="https://www.example.com" target="_blank">Example Site 2</a></p>
  
  ```
- **Essence**: `<a>` is the anchor tag used to define hyperlinks. `href` attribute contains the URL of the link. `target="_blank"` opens the link in a new tab/window.

#### Step 5: Add Style and Emphasis

- **Task**: Emphasize some text and add a horizontal line.
- **Code**:
  ```html
  <p>I love learning about <strong>HTML</strong> and <em>web development</em>.</p>
  <hr>
  ```
- **Essence**: `<strong>` makes text bold, indicating it's of strong importance, while `<em>` italicizes text, indicating emphasis. `<hr>` creates a thematic break in the form of a horizontal line, often used to separate content sections.

#### Step 6: Test and Experiment

- **Task**: Save your HTML file and open it in a web browser to see your work. Try modifying elements, adding more content, or rearranging sections.
- **Code**: No additional code, just experimentation.
- **Essence**: Testing and iterating are key parts of web development. Viewing your page in a browser lets you see how your code translates into a webpage. Experimentation helps you understand how different elements interact and affect the layout and style.


> For fun: Take a screenshot of your code and the final output in the browser and post on X (Twitter) and tag @learninbits as well as @ehoneahobed so we can all follow your progress and cheer you on.

# Lists
Lists are a fundamental part of HTML, allowing for the organization of content into an ordered or unordered format. They are widely used for things like menus, steps, features, and more. There are primarily three types of lists in HTML: unordered lists, ordered lists, and description lists.

### Unordered Lists (`<ul>`):

- **Purpose**: To create a list of items without any particular order.
- **Element**: `<ul>` is the container for the unordered list, and each item within the list is enclosed in an `<li>` (list item) tag.
- **Common Use**: For bullet lists where the order of items doesn't matter.
- **Appearance**: By default, unordered lists are rendered with bullet points.

```html
<ul>
  <li>Apples</li>
  <li>Bananas</li>
  <li>Oranges</li>
</ul>
```

### Ordered Lists (`<ol>`):

- **Purpose**: To create a list of items in a specific order.
- **Element**: `<ol>` is the container for the ordered list, and similar to `<ul>`, each item is placed within an `<li>` tag.
- **Common Use**: For numbered instructions, rankings, or any list where the sequence is important.
- **Appearance**: By default, ordered lists are rendered with numbers.

```html
<ol>
  <li>First do this.</li>
  <li>Then do this.</li>
  <li>Finally, do this.</li>
</ol>
```

### Description Lists (`<dl>`, `<dt>`, and `<dd>`):

- **Purpose**: To pair terms with their descriptions.
- **Elements**:
  - `<dl>`: Description List container.
  - `<dt>`: Term (name) in the description list.
  - `<dd>`: Description of the term.
- **Common Use**: For glossaries, metadata, or any other type of list that involves name-value pairs.
- **Appearance**: Usually, terms are on their own line, and descriptions are indented.

```html
<dl>
  <dt>HTML</dt>
  <dd>Hypertext Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

### General Notes on Lists:

- **Nesting**: Lists can be nested within each other. For example, an `<ul>` or `<ol>` can contain another `<ul>`, `<ol>`, or `<dl>` to create sublists.
- **Attributes**: Lists can have attributes like `class`, `id`, `style`, etc., for styling purposes.
- **Accessibility**: Properly used lists are good for accessibility as they provide structure that can be easily navigated by screen readers.

Lists are versatile and widely used in HTML for a variety of content structures. They are essential for creating organized, readable, and accessible content on the web. Whether you're making a simple bullet list of items, a complex nested structure, or pairing terms with definitions, HTML lists provide the structure you need.
