# Basic HTML Elements
Just as you learned earlier, to master HTML means know the various elements, how and when to use them. There are some elements that are very basic and are commonly used.

Let's start by taking a look at some of these popular elements especially those that are used in marking up text.

### Heading
In designing your webpages, you may want to have some portion of your documents to serve as headings (titles). In HTML, there are special elements to indicated headings. The heading element is indicated with a number from 1 to 6 where one is the biggest and six is the smallest.

<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>

Try by adding headings to your `home.html` page.

```
<!DOCTYPE html>
<html>
    <head>
        <title>HTML & CSS Bootcamp 2024 - Batch 1</title>
    </head>
    <body>
        <h1>Heading One looks like this</h1>
        <h2>Heading Two looks like this</h2>
        <h3>Heading Three looks like this</h3>
        <h4>Heading Four looks like this</h4>
        <h5>Heading Five looks like this</h5>
        <h6>Heading Six looks like this</h6>
        
        This is my first webpage and I can't wait to master HTML and CSS!
    </body>
</html>
```

Refresh your web browser and see the new changes take place.

![Alt text](image-15.png)

> NB: It is worth noting that `H1` should used only once on any webpage and that should be for the most important thing on the page which using happens to be the main topic/title the webpage is about. 

### Paragraph
Also, most texts that you will write in your webpage must be captured in paragraphs. For such, you will need to use the paragraph element.

```
<p></p>
``` 

Improve the content on your `home.html` by capturing the text in a paragraph element.

```
<!DOCTYPE html>
<html>
    <head>
        <title>HTML & CSS Bootcamp 2024 - Batch 1</title>
    </head>
    <body>
        <h1>Heading One looks like this</h1>
        <h2>Heading Two looks like this</h2>
        <h3>Heading Three looks like this</h3>
        <h4>Heading Four looks like this</h4>
        <h5>Heading Five looks like this</h5>
        <h6>Heading Six looks like this</h6>
        
        <p>This is my first webpage and I can't wait to master HTML and CSS!</p>
    </body>
</html>
```
When you save this and refresh your browser, noting changes visually but now your browser is fully aware that the text is in a paragraph element. You will appreciate the importance of such things when you start learning about styling your webpage with CSS.

![Alt text](image-16.png)


### Sectioning (Block vs inline elements)
More often than not, you will want to divide the content on your webpage into several different sections. For example, you may want to have:

- Header
- Left sidebar
- Main section
- Right sidebar
- Footer

Even apart from these main part, you may sometimes want to separate concerns in one main part or create subsections for your document. Imagine this as what you do in the formal letter writing where you have addresses, salutations, subject/title, introduction, main body, conclusion, and subscription.

Imagine if your webpage was supposed to just display a formal letter that you have written, you may want to create all the respective sections.

To do this, there aare some generic elements that we can use. Two of the common ones are: `div` and `span`.

The `div` element is a block element which means that when used, it takes up the whole line that it is on and pushes any adjacent element to the bottom (unless overriden with CSS).

The `span` element on the otherhand is an inline element which means that it takes up only the space it covers and allows all adjacent element to be as they originally were and **not force** any element down.

The `span` and `div` element may seem not to do much visually on your webpage but they are very significant especially when it comes to styling the page.


**Examples**

Using div for sectioning:

```
<!DOCTYPE html>
<html>
<head>
    <title>My Webpage</title>
</head>
<body>

    <div id="header">
        <h1>My Website</h1>
    </div>

    <div id="navigation">
        <p>Link 1 | Link 2 | Link 3</p>
    </div>

    <div id="content">
        <h2>Welcome to my website</h2>
        <p>This is a paragraph in the main content area.</p>
    </div>

    <div id="footer">
        <p>Footer information</p>
    </div>

</body>
</html>

```
In this structure, each <div> creates a new block-level section for the header, navigation, content, and footer.

Using <span> for Inline Emphasis
`<span>` elements are used for styling or targeting small pieces of text or other inline elements without affecting the surrounding content. Here's how you might use `<span>`:

```
<p>Welcome to <span style="color:blue">Blue City</span>! Enjoy your stay.</p>
```

Here, only "Blue City" will be colored blue, and the rest of the sentence remains unaffected. `<span>` doesn't break the flow of text and doesn't start on a new line.

NB: Don't worry if you don't understand the role the attributes `id` and `style` that were used. You will get to understand them soon.

**Combining Both in a Practical Scenario**
Imagine you're creating a section of a webpage for a user profile. You might use <div> to create the section and <span> to highlight certain parts of the text:

```
<div class="user-profile">
    <h2>User Profile</h2>
    <p><strong>Name:</strong> <span class="name">Jane Doe</span></p>
    <p><strong>Occupation:</strong> <span class="occupation">Web Developer</span></p>
    <p><strong>Hobbies:</strong> <span class="hobbies">Coding, Hiking</span></p>
</div>
```

### Formatting text (Bold, Italic, Underline)
There are times that you may want to bolden some part of your text or make some italic, underline some or lay some emphasis on some parts.

Here are tags that you can use:

```
Bold: <b></b> or <strong></strong>
Italic: <i></i>
Underline: <u></u>
Emphasize: <em>
```

### Others (Line breaks, horizontal lines, Code, Preformatted text)
As you continue to learn HTML, you'll come across various elements that allow you to structure and present your content more effectively. Let's discuss some of these: line breaks, horizontal lines, code, and preformatted text.

#### Line Breaks (`<br>`)
When you want to add a single line break without starting a new paragraph, you use the <br> element. This is particularly useful for addresses or poems where the line division is significant.

```
<p>
    1. This is the first line without line break,
    And this is the second.
</p>

<p>
    2. This is the first line with line break,<br>
    And this is the second.
</p>
```

If you add the example above to your `home.html` and preview it in the browser, you will get an output like this:

![Alt text](image-17.png)

You observe that even though you wrote the phrase `And this is the second` on the second line, it turned out to be on the same line as the first one in your first paragraph.

However, on the second paragraph, the second line was forced to the next line because you used a line break.

#### Horizontal Lines (`<hr>`)
The <hr> element represents a thematic break between paragraph-level elements (e.g., a change of scene in a story, a shift of topic within a section). It typically manifests as a horizontal line.

```
<p>First section of the text.</p>
<hr>
<p>Second section of the text.</p>
```

Sample code like above will produce an output like this:

![Alt text](image-18.png)

#### Code (`<code>`)
The `<code>` element is used to display a single line of code. It's an inline element and typically presented in the browser's default monospace font.

```
<p>
    To install the package, run <code>npm install package-name</code> in your terminal.
</p>
```

![Alt text](image-19.png)

In this example the way `npm install package-name` is displayed is a bit different from the other surrounding text. This is because the `<code>` element changes the font of its content.

#### Preformatted Text (`<pre>`)
When you want to display text exactly as it's written in the HTML file, including spaces and line breaks, use the `<pre>` element. It's often used for code blocks because it preserves both spaces and line breaks.

```
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks.
</pre>
```

Here is the output:

![Alt text](image-20.png)


NOTE: All these elements are fundamental in HTML and are often used to enhance the readability and structure of the content. As you become more familiar with HTML and CSS, you'll learn how to style these elements to fit the design of your website.

### Exercise: Create a Personal Web Page
Objective: Create a simple personal web page using the HTML elements you've learned.

Requirements:
- Page Title: Use `<h1>` to add a main title to your page: "My Personal Web Page".
- Subsections with Headings: Use `<h2>` to create at least three subsections: About Me, My Skills, and My Hobbies.
- Paragraphs: In each subsection, add a brief description using <p> tags.

- Styling Text:
    - Within your paragraphs, make your name bold using `<b>` or `<strong>`.
    - Emphasize your job title or a key hobby using `<em>` or `<i>`.
    - Underline a significant achievement or an important skill using <u>.

- Code Snippet: Use the `<code>` tag to include a small snippet of code you're proud of or interested in. Use `<pre>` if it's multiple lines.
- Horizontal Line: Use `<hr>` to separate content between the sections.
- Line Breaks: Use `<br>` to add space where necessary, like in addresses or poems.
- Division and Span: Use `<div>` to contain each section (About Me, My Skills, My Hobbies) and use `<span>` to highlight any particular text within your paragraphs that you want to style later with CSS.

Instructions:
- Setup: Create an HTML file named `mysite.html`.
- Structure: Follow the structure given in the requirements. Start with your page title and then create each subsection with the respective headings and content.
- Content: Be creative with your content! Write about yourself, your skills, and what you enjoy doing.
- Testing: Open your HTML file in a web browser to test how it looks. Make sure all the HTML elements are properly displayed.

# Comments
Sometimes when writing your code, you want to add some comments on what the code does so that when you come back to it at a later time you will still understand what that code is for.

The question therefore is how to achieve this in programming. Interestingly enough every programming language has a unique way to write comments. For now you will learn how to add comments to your HTML code.

Comments in HTML are used to insert notes, explanations, or warnings in the code that are not displayed in the browser. They are extremely useful for developers to document the code, make it more readable, or explain complex parts of the markup. Comments can also be used to temporarily disable code that you don't want to run.

Here is the syntax for comments in HTML:

```
<!-- This is a comment in HTML -->
```

So, if you want to start a comment, you will write `<!--` followed by the actual comment and finally end it with `-->`

Anything between `<!-- and -->` will be ignored by the browser and will not render as part of the web page. You can place comments in your HTML code wherever you want to annotate or explain something. They can be single-line or extend over multiple lines.
