## HTML Basics
HTML (HyperText Markup Language) is the code that is used to structure a web page and its content. For example, content could be structured within a set of paragraphs, a list of bulleted points, or using images and data tables.

HTML is a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. 

For example, this is how we define a paragraph in html using `<p>` element. 
    
    <p>My cat is very grumpy</p>

## Anatomy of an HTML element
![](./images/html-element-anatomy.png)

The main parts of our element are as follows:

1. `The opening tag`: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.
2. `The closing tag`: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
3. `The content`: This is the content of the element, which in this case, is just text.
4. `The element`: The opening tag, the closing tag, and the content together comprise the element.

Elements can also have attributes that look like the following:

![](./images/html-element-attr.png)

Attributes contain extra information about the element that you don't want to appear in the actual content. Here, class is the attribute name and editor-note is the attribute value. The class attribute allows you to give the element a non-unique identifier that can be used to target it (and any other elements with the same class value) with style information and other things.

### Nesting elements
You can put elements inside other elements too — this is called nesting. 

    <p>My cat is <strong>very</strong> grumpy.</p>

You do however need to make sure that your elements are properly nested.

    <p>My cat is <strong>very grumpy.</p></strong> (Wrong)

### Void elements
Some elements have no content and are called void elements. Take the <img> element that we already have in our HTML page:

    <img src="images/firefox-icon.png" alt="My test image" />

This contains two attributes, but there is no closing </img> tag and no inner content. This is because an image element doesn't wrap content to affect it. Its purpose is to embed an image in the HTML page in the place it appears.

## Anatomy of an HTML document

In this section, we'll look at how individual elements are combined to form an entire HTML page.

    <!DOCTYPE html>
    <html lang="en-US">
    <head>
        <meta charset="utf-8" />
        <meta name="viewport" content="width=device-width" />
        <title>My test page</title>
    </head>
    <body>
        <img src="images/firefox-icon.png" alt="My test image" />
    </body>
    </html>

1. `<!DOCTYPE html>` — doctype. It is a required preamble. In the mists of time, when HTML was young (around 1991/92), doctypes were meant to act as links to a set of rules that the HTML page had to follow to be considered good HTML, which could mean automatic error checking and other useful things. However, these days, they don't do much and are basically just needed to make sure your document behaves correctly. 
2. `the <html>` element. This element wraps all the content on the entire page and is sometimes known as the root element. It also includes the lang attribute, setting the primary language of the document.
3. `the <head>` element. This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes things like keywords and a page description that you want to appear in search results, CSS to style our content, character set declarations, and more.
4. `<meta charset="utf-8">` — This element sets the character set your document should use to UTF-8 which includes most characters from the vast majority of written languages. Essentially, it can now handle any textual content you might put on it. There is no reason not to set this, and it can help avoid some problems later on.
5. `<meta name="viewport" content="width=device-width">` — This viewport element ensures the page renders at the width of viewport, preventing mobile browsers from rendering pages wider than the viewport and then shrinking them down.
6. `the <title>` element. This sets the title of your page, which is the title that appears in the browser tab the page is loaded in. It is also used to describe the page when you bookmark/favorite it.
7. `the <body>` element. This contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, playable audio tracks, or whatever else.

## HTML Comments
Anything in HTML between <!-- and --> is an HTML comment. The browser ignores comments as it renders the code. In other words, they are not visible on the page - just in the code. HTML comments are a way for you to write helpful notes about your code or logic.

    <!-- 4 heading levels: -->

### Headings
Heading elements allow you to specify that certain parts of your content are headings — or subheadings. HTML contains 6 heading levels, <h1> - <h6>.

    <!-- 4 heading levels: -->
    <h1>My main title</h1>
    <h2>My top level heading</h2>
    <h3>My subheading</h3>
    <h4>My sub-subheading</h4>

## Paragraphs
As explained above, <p> elements are for containing paragraphs of text.

    <p>This is a single test paragraph</p>

## Lists
A lot of the web's content is lists and HTML has special elements for these. Marking up lists always consists of at least 2 elements. The most common list types are ordered and unordered lists:

1. <b>Unordered</b> lists are for lists where the order of the items doesn't matter, such as a shopping list. These are wrapped in a `<ul>` element.
2. Ordered lists are for lists where the order of the items does matter, such as a recipe. These are wrapped in an `<ol>` element.

Each item inside the lists is put inside an `<li>` (list item) element.

For example, if we wanted to turn the part of the following paragraph fragment into a list

    <p>
        At Mozilla, we're a global community of technologists, thinkers, and builders working together…
    </p>

We could modify the markup to this

    <p>At Mozilla, we're a global community of</p>

    <ul>
    <li>technologists</li>
    <li>thinkers</li>
    <li>builders</li>
    </ul>

    <p>working together…</p>

## Links

Links are very important — they are what makes the web a web! To add a link, we need to use a simple element — <a> — "a" being the short form for "anchor". 

    <a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>