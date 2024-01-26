## Introduction to HTML
For any website that you see on the internet, there is some HTML code behind the scene that is being rendered for you to see what you see. 

HTML stands for HyperText Markup Language.

HTML is a markup language that is use to structure text and other types of media. To create a complete webpage, you will usually combine HTML with a styling language like CSS and scripting language like JavaScript.

The HTML part of the webpage is what is responsible for the actual content of the webpage. So, if a webpage has some text, images, videos, etc then it is the doing of HTML.

HTML is made up of two major things: **Elements and Attributes** and you will get to know what these are in a jiffy.

### What is an Element?
To make a particular content to appear on your webpage, you will wrap it within a specific element.

An element is made up of an _opening_ and a _closing tag_. What are these tags then?

**Tags** are just keywords that are enclosed in angle brackets (<>) which carry specific meaning which is understood by browsers.

- Opening tag: Looks like this `<tag name>`
- Closing tag: Looks like this `</tag name>`

> NB: The difference between an opening tag and a closing tag is the forward slash that is used in the closing tag.

An element therefore looks like <tagname>The type of content goes here</tagname>

It is important to note that we have some elements which can be used without necessarily having content in between the tags. You can say that they are empty but technically, we call such elements, **self-closing elements**. For such elements, there is no need to bring the closing tag since they have no content (Remember that you would ideally have written the content right after the opening tag and then use the closing tag to show the end of that content.)

There are times that you may want to modify the behaviour of an element. You can do this with what we call **attributes**. These are key-value pairs that can be introduced in the opening tag.

> eg: `<tagname attributename=value>Content of element goes here</tagname>`

An element may have multiple attributes.

There are elements for various purposes including: texts, forms, images, videos, sectioning, etc.

Knowing HTML means knowing the various elements, when and how to use them.

We will introduce the basic HTML elements in subsequent lessons.

## Checking the Source Code of a Webpage
The best way to introduce you to what an actual HTML code looks like is to have you look at the code for an existing website.

It is going to look like a lot but get scared. The basic information that you have been equipped with is all you need to know to understand the code.

Here are the key terms that you came across previously that you need to appreciate to understand any HTML code:

1. Opening tag
2. Closing tag
3. Content
4. Attribute
5. Element

The whole web page is made up of a combination of elements and as you know by now, an element is made up of an opening and closing tags and may contain some contents as well as some attributes.

### How to see the HTML code of a webpage
If you are on any website and would want to see the HTML source code for that page, right click on it and click on the "View Page Source".

![Alt text](image.png)

**Exercise:** 
Visit the webpage for this bootcamp: https://learninbits.com/html-css-bootcamp/ and check out the source code to help you answer these questions.

1. List at least 5 of the various tags that you find in the source code and take note of the content of each

2. List at least 5 different attributes with their respective values


After doing this, you will now be ready to write your own HTML code.

# Creating your first Webpage
Are you ready to create your first webpage?

If you are then let's get to it.

### What you need to be able to create a webapge
There are two basic things that you require:
- A code editor (to write the HTML code)
- A browser (to observe the webpage you create)

#### 1. Code Editors
Code editors are software that you use to write code. If you have ever used a text editor or processor like Microsoft Word or Notepad then you can think of code editors as similar tools but specialized for code writing.

There are a lot of code editors available such that it sometimes even becomes difficult to choose a particular one. You just have to choose one of them and stick with it.

Popular examples of code editors include:
- VS Code, Sublime Text, Atom

If you choose to go with any of the above then you have to download it and install it on your computer.

My personal favorite is VS Code. Recently, a web version of VS code was released. This means that you can either [download and install VS code](https://code.visualstudio.com/download) or just make use of [VS code](https://vscode.dev/) in your browser.

There are other online available code editors that you can use without having to install anything on your computer. For the sake of the exercises and projects in this bootcamp, you will be required to make use of some of these online text editors.

To get started, you will be using [Codesandbox](https://codesandbox.io/). Visit the site and create an account with [Codesandbox.io](https://codesandbox.io/). Every code that you write will be easily accessible which will serve as your portfolio by the time you have completed the bootcamp. It also ensures that you always have access to the code that you wrote even if you do not have access to the computer that you used.

Other similar platforms that you can also explore include:
- [Codepen](https:///codepen.io)
- [Replit](https://replit.com)



#### 2. Browsers
Once you have created your webpage, you will need a software to open it with. That is where browsers come in. You may be familiar with a number of browsers out there. Some of the popular ones are: Google Chrome, Moxilla Firefox, Microsoft Edge, Safari, Opera Mini, etc.

Amongst these, Chrome and Firefox have become developers favorite when it comes too building websites or web apps. For the purpose of the bootcamp, you are recommended to stick to Google Chrome. Hence, if you don't already have Google Chrome installed on your computer, go ahead and [download and install Google Chrome](https://www.google.com/chrome/dr/download/).

### Creating your first webpage
Let's begin by setting up **Codesandbox** for our work. I hope you have already created an account, if not then go ahead and [create your account now](https://codesandbox.io/).

Now, go ahead and sign in into Codesandbox. You will be greeted with an interface that looks like this:

![Alt text](image-1.png)

- Click on "Create a Sandbox" or at the top right corner, click on create and it brings you the options from which you can proceed to click on "Create a Sandbox".

![Alt text](image-2.png)

- The next step is to choose a template. Go ahead and click on "HTML + CSS".
![Alt text](image-3.png)

- Proceed to give your sandbox a name (use: learninbits-html-css-bootcamp)

![Alt text](image-4.png)

So, go ahead and update the name to "learninbits-html-css-bootcamp" like shown below and when you are done, click the `Create Sandbox` button.

![Alt text](image-5.png)

Afterwards, you will have an interface like this:

![Alt text](image-8.png)

As you can see on the left side, you will be working in the directory called `NODEBOX`. Also, you may have realized that there are three different files in that directory and each of them has a different ending (extension).

The text that comes after the dot in the name of the file is known as the file extension and it is what determines the file type. So, to create HTML files, you will have to add the extension `.html` to the name of the webpage.

![Alt text](image-9.png)

To create a new file, take a look at the icons that are to the right of `NODEBOX` and you will find the add file icon. Click on that and name your file `home.html`.

![Alt text](image-10.png)

Once created, the file opens to the right. Congratulations if you have gotten this far.

## Writing your first HTML Code
Do you remember the basic template for writing formal letters

```
- Sender's Address
- Date
- Recipient's Address
- Salutation
- Subject / Title
- Introduction
- Main Body
- Conclusion
- Signature
- Subscription
```

At least that was what we were taught in high school. What does this gotten to do with writing your first HTML code, you ask?

Well, there is a specific structure that your code needs to be for the browser to recognize and render it the right way without any errors.

```
- Document type declaration: <!DOCTYPE html>
- HTML: Root element <html>
- Head: <head>
- Body: <body>
```

So, in your `home.html` file, go ahead and write your first code as shown below:

```
<!DOCTYPE html>
<html>
    <head></head>
    <body></body>
</html>
```

A couple of things to take note of:
- Both the `head` and `body` elements are put within the `html` element.
- 3 main elements were used above: (HTML element, head element, body element)
- For now we are yet to put content in both the head and body elements.

The content of an element can also be another element. This is called nesting of elements. For example, we have nested both the head and body elements within the html element.

When nesting elements, tags should be closed in the reverse order of which they were opened.

Essentially all the code you will be writing will go into the head and body elements. 

It is important however to know that the content of the head element won't show up on the webpage. It is only the content of the body element that shows up on the webpage.

Let's focus on the head element and let's discover some of the common elements that can be nested into the head element.

- `<title></title>`
- `<style></style>`
- `<link></link>`
- `<script></script>`
- `<meta />` (This is a self closing tag)

Don't worry so much about what each of these elements do because you will get to understand them soon.

For now, let's talk about the title element.This element contains the content that will be displayed in the browsers tab and also in search engines.

For example, in the image below, you can see that the tab contains the phrase "HTML & CSS Bootcamp 2024 -".

This means that if you inspect the source code for the page you will find that the title element contains that same phrase.

```
<title>HTML & CSS Bootcamp 2024 -</title>
```

![Alt text](image-11.png)

Go ahead and add the title element to your HTML code. Remember that the title element is contained in the head element.

```
<!DOCTYPE html>
<html>
    <head>
        <title>HTML & CSS Bootcamp 2024 - Batch 1</title>
    </head>
    <body></body>
</html>
```

To finish this first HTML code off, let's add some content into the body element so that something can be displayed in our browser when we observe it.

Add the following text as the content of your body element:

```
This is my first webpage and I can't wait to master HTML and CSS!
```

This means that your final code should look like this:

```
<!DOCTYPE html>
<html>
    <head>
        <title>HTML & CSS Bootcamp 2024 - Batch 1</title>
    </head>
    <body>
        This is my first webpage and I can't wait to master HTML and CSS!
    </body>
</html>
```

Now go ahead and save the file (You can use CTRL + S).

## Observing your webpage
As discussed earlier, you need a browser to render your HTML code into a human readable and appealing webpage. Note that when a browser renders your code, the tags will not show. The tags together with the various attributes are the set of instructions that the browser interpretes and produces the final output which is appealing to humans.

If you used a code editor installed on your computer then you have to check for the location of the file and right click on it and select open with and choose Chrome. This will display the your webpage in the browser.

If you are using Codesandbox as recommended for this bootcamp, you have the browser instance for previewing the code to your right hand side.

Currently, you have something else (the default index.html file being shown in the preview).

![Alt text](image-12.png)

You need to update the preview url to that of your own document. Since your HTML file was called `home.html`, just add that to the end of the current URL. For the screenshot attached, the new URL will therefore become:

```
https://mqvpgx.csb.app/home.html
```
![Alt text](image-13.png)

As you can see, only the content within the body element is showing on the webpage. It is worth noting that the title isn't showing in the preview tab but that is just how Codesandbox behaves. If you want to see it, you can copy your URL and paste it in any browser.

As you can see below, when the URL was copied into a new tab, the title showed in the tab and the content of the body shows in the webpage.

![Alt text](image-14.png)
