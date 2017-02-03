<link href='https://fonts.googleapis.com/css?family=Lato:400' rel='stylesheet' type='text/css'>

<style>
.major-key {
  background-color: rgba(255, 215, 48, 0.4);
  padding: 2px 0;
  transition: 0.1s ease background-color;
}

.major-key:hover {
  background-color: rgba(255, 215, 48, 0.7);
}

img {
    display: block;
    margin: 0 auto;
    max-width: 100%;
}

a {
    color: #0088bd !important;
}

a:visited {
    color: #0048ad !important;
}

a:hover {
    color: #06f !important;
}

.extra-cool-text {
  color: #42cbad;
  font-weight: 700;
  line-height: 40px;
}

.ALMIGHTY-GOLDEN-RATIO {
    color: rgb(255, 215, 48) !important;
}

.ALMIGHTY-GOLDEN-RATIO:visited {
    color: rgb(255, 215, 48) !important;
}

.font-size-1 {
  font-size: 10px;
  padding: 0;
}

.font-size-2 {
  font-size: 18px;
  padding: 0.25rem 0;
}

.font-size-3 {
  font-size: 32px;
  padding-bottom: 1rem;
}

.line-height-1 {
  line-height: 1em !important;
}

.line-height-2 {
  line-height: 2em !important;
}

.font-weight-1 {
  font-weight: 400;
}

.font-weight-2 {
  font-weight: 700;
}

.font-weight-3 {
  font-weight: 900;
}

.font-style-1 {
  font-style: italic;
}

.font-family-1 {
  font-family: Times New Roman;
}

.font-family-2 {
  font-family: Helvetica;
}

.font-family-3 {
    font-family: Lato;
}

.color-1 {
  color: #000;
}

.color-2 {
  color: #00f;
}

.color-3 {
  color: rgb(42, 136, 252);
}

</style>

<a id="top"></a>
# From Zero to Website

*Learn to build your own personal website! No programming experience required.*

Written and developed by [Evan Tarrh](http://evan.land) and [ADI](adi).

<a href="#top" class="top" id="getting-started">Top</a>
## Getting Started

### What will I learn?

We'll cover the fundamentals of HTML, CSS, and JavaScript. Once we've covered the basics, we'll use GitHub to deploy a personal site for the whole world to see.

### What do I need to get started?


Before going through this tutorial, **do these things**:

-   Register on [GitHub](//github.com). Plus, get your [student
    developer pack](//education.github.com/pack)! It will serve
    you well.
-   Download [Sublime Text](//www.sublimetext.com/3).
-   Install and set up
    [Git](https://help.github.com/articles/set-up-git/). In that guide,
    all you have to do is the four steps inside “Setting up Git”, but
    you can also follow the steps for authenticating with GitHub if
    you're feeling adventurous.

### OK, I'm ready!

Then let's go!

<a href="#top" class="top" id="table-of-contents">Top</a>
## Table of Contents

-	[Level 1: HTML](#html)
    -	[1.1 What does HTML look like?](#intro-html)
    - [1.2 What should an HTML file look like?](#files)
    - [1.3 How do we organize HTML files?](#structure)
    - [1.4 How do we know what's going on in the browser?](#inspector)
    - [1.5 HTML terms you should know](#terms-html)
    - [1.6 A short project](#project-html)
- [Level 2: CSS](#css)
    - [2.1 What is CSS? What does it look like?](#intro-css)
    - [2.2 Selectors](#selectors)
    - [2.3 How can I customize text with CSS?](#text)
    - [2.4 How do colors work in CSS?](#colors)
    - [2.5 How do I position elements on a page?](#position)
    - [2.6 How do colors work in CSS?](#colors)
    - [2.7 How do I put CSS in my HTML file?](#linking-css)
    - [2.8 CSS terms you should know](#terms-css)
    - [2.9 Explore the wonderful world of CSS](#project-css)
- [Level 3: JavaScript](#js)
    - [3.1 JavaScript in the console](#console)
    - [3.2 JavaScript variables](#console)
    - [3.3 Grouping values with arrays](#arrays)
    - [3.4 jQuery is your friend](#jquery)
    - [3.5 Using jQuery selectors](#selectors-jquery)
    - [3.6 Handling events with jQuery is a major key](#events)
    - [3.7 Manipulating CSS with jQuery](#jquery-css)
    - [3.8 Animating things with jQuery](#animation)
    - [3.9 `$(document).ready`](#document-ready)
    - [3.10 JS terms you should know](#terms-js)
    - [3.11 Very Serious Assignment](#project-js)
- [Level 4: Git](#git)
    - [4.1 Navigation in the terminal](#terminal)
    - [4.2 Creating and cloning your first repo](#intro-git)
    - [4.3 Committing changes to a project](#committing)
    - [4.4 Git terms you should know](#terms-git)
    - [4.5 Do things with Git](#project-git)
- [Level 5: Next Steps](#next-steps)
    - [5.1 Using Flask to build web applications](#flask)
    - [5.2 Customizing your domain](#domains)
    - [5.3 CSS Media Queries](#responsive)
    - [5.4 Better JavaScript](#better-js)
    - [5.5 Favicons](#favicons)
    - [5.6 Google Analytics](#ga)
    - [5.7 Bootstrap](#bootstrap)

------------------------------
<a href="#top" class="top" id="html">Top</a>
## Level 1: HTML

HTML is the language of the Internet. Whenever you visit a website, what
you see is the result of HTML being interpreted and rendered by your
browser.

<a id="intro-html"></a>
### 1.1 What does HTML look like?

It's simple!

    <p>It's simple!</p>

HTML is simply the content you see on the screen, with extra markup
around it to help format it. In the example above, the
`<p>` is an **opening tag** that denotes the start of a
paragraph, and the `</p>` closes the paragraph. The whole
paragraph can be referred to as an **element**.

HTML is more than just paragraphs, though. Let's get familiar with some
more HTML elements!

<a id="headers"></a>
#### Headers

One of the best ways to create hierarchy is with **headers**. At the top
of this page, the text "DevFest Beginner Development Track" is actually an `h1`, so the code
looks like `<h1>DevFest Beginner Development Track</h1>`.

`h1`'s are the biggest options for headers, but there are
also `h2`'s and `h3`'s, all the way down to
the rarely-used `h6`. For example, the bold "Headers" a
couple of lines above is an `h4`.

<a id="links"></a>
#### Links

We can use **anchor tags** to link to other pages!

    <a href="http://jumpman.space">Jumpman Jumpman Jumpman</a>

The `href` attribute contains the URL that the link will
send you to, and the content inside the tags is what the user actually
sees. So, the code above ends up producing this:

[Jumpman Jumpman Jumpman](http://jumpman.space)

If you're linking to another website, it's important to always include
the `http://` at the beginning of the link inside the
`href`.

However, <span class="major-key">when you link to a different page on
the same website, you should always omit both the
`http://` and the base URL</span>—so, for example, if I
wanted to link to `learn.devfe.st/data-science`, the tag
should look like this: `<a href="/data-science">`. This
means that if you ever just want to link to the homepage (e.g.
`learn.devfe.st`), the correct `href` is simply
`href="/"`.

Note that the `href` goes inside the tag itself! This
isn't the only element for which this happens. Another great example is
the `<img>` tag!

<a id="images"></a>
#### The `<img>` tag

It's actually really easy to put pictures on websites—there's a tag for
that!

<img src="http://imgs.xkcd.com/comics/tags.png">

    <img src="http://imgs.xkcd.com/comics/tags.png">

Note that `<img>` tags do not need need a closing tag,
i.e., `</img>`.

Also, note that the source of the image (a URL specifying the location
of the image) goes inside the tag itself. This isn't the only
**attribute** that can be specified inside the tag: we can also set the
height and/or width of the image like this!

    <img src="http://imgs.xkcd.com/comics/tags.png" width="100%">

    <img src="http://imgs.xkcd.com/comics/tags.png" height="300px">

There are several valid formats for these `height` and
`width` attributes, which we'll cover in more detail in
our section on CSS.

<a id="divs"></a>
#### The container element: `<div>`

`<div>`'s are container elements. They offer a way to
organize different HTML elements by **nesting**. In other words, a
`<div>` will almost always contain other elements inside
it, like so:

    <div>
        <img src="http://imgs.xkcd.com/comics/tags.png" width="300px">
    </div>

Note that the `img` is indented in this code block. It's
common practice to indent whenever an HTML element is **nested** inside
another one. When this happens, we refer to the `div` as
the **parent** element, and the `img` as the **child**.

`<a>` tags are another great example of an element that involves nesting. An `<a>`
tag should always be nested inside a `<p>`, like so:

    <p>
      Check out this cool <a href="https://youtu.be/ZerV5WcnBAo?t=2m19s">computer stuff</a>!
    </p>

That HTML will end up looking like this:

> Check out this cool [computer stuff](https://youtu.be/ZerV5WcnBAo?t=2m19s)!

As far as divs go, we'll learn more about them when we move on to styling
our pages with CSS. For now, we can just think of them as organizational tools, to help separate our HTML into meaningful sections.

<a id="typographical-elements"></a>
#### Typographical elements: `<strong>` and `<em>`

For anyone who likes typography, this is the fun stuff! You can use tags
to make your type **bold** or *italicized*.

    <strong>I'm bold!</strong>

    <em>I'm italicized!</em>

    <strong>
        <em>I'm bold and italicized!</em>
    </strong>

    <em>
        <strong>I'm bold and italicized, too! The order doesn't matter here.</strong>
    </em>

This HTML will be rendered as:

> **I'm bold!**

> *I'm italicized!*

>_**I'm bold and italicized!**_

>_**I'm bold and italicized, too! The order doesn't matter here.**_

<a id="files"></a>
### What should an HTML file look like?

OK, we've already learned a lot! There are more useful HTML elements out
there, but we still have a pretty good idea of what HTML looks like.
Now, let's focus on how to use HTML in practice.

Here's a very minimal skeleton. We can fill it out later once we start
building our own pages!

    <!DOCTYPE html>
    <html>
        <head>
            <!-- This is a comment. -->

            <title>Wow!</title>
        </head>
        <body>
            <!-- Put all content here. -->
        </body>
    </html>

Check it out! Let's look at this file line-by-line to understand it.

-   `<!DOCTYPE html>`

    Every HTML file must have exactly this as its first line. Otherwise,
    your browser won't know how to interpret the file.

-   `<html>`

    Remember how you can nest HTML elements? Well, it turns out that
    every HTML file is nested inside one `html` element!
    This line of code is almost always the second line of code inside an
    HTML file, and it must contain exactly two children:
    `head` and `body`.

-   `<head>`

    The `head` element contains information about the HTML
    page that is important, but shouldn't be rendered inside your
    browser alongside all the content. For example, this is how your
    browser knows what text to put in the tab (for this website, “From
    Zero to Website”), or the little icon next to it (the green J).

-   `<!-- This is a comment -->`

    **Comments** can help clarify confusing sections of code. They're a
    useful way to explain your code to someone else (most often, the
    “someone else” ends up being you 2 months later, so be nice to your
    future self).

    Comments must begin with `<!--` and end with
    `-->`.

-   `<title>Wow!</title>`

    The `title` is that small blob of text that's
    displayed in your browser's tab. It won't affect anything else on
    the page.

-   `</head>`

    Closing the `head` tag. The head must be closed before
    the body begins. …That's a weird sentence.

-   `<body>` and `</body>`

    The `body` is where all of the content on the
    page goes. All of the tags we talked about
    before—`p`'s, `div`'s,
    `img`'s—go here!

That's what a basic HTML file should look like! We're only missing one
thing—the name of the file. The only rule is that the file must end in
`.html`. However, there is a special case:
`index.html`. This will fold in nicely to our next
mini-topic: the directory structure for websites.

<a id="structure"></a>
### How do we organize HTML files?

This might be a little complicated, and it's hard to explain without
looking at an example. So, let's use this website as an example! The
**root directory** of this website is a folder called
`learn.devfe.st/`, and it contains seven HTML files. Here are the
files and their respective URLs:

-   `index.html` : `learn.devfe.st/`
-   `index.html` : `learn.devfe.st/beginner-dev/index.html`
-   `index.html` : `learn.devfe.st/data-science/index.html`
-   `index.html` : `learn.devfe.st/game-dev/index.html`
-   `index.html` : `learn.devfe.st/ios/index.html`
-   `index.html` : `learn.devfe.st/product/index.html`
-   `index.html` : `learn.devfe.st/webdev/index.html`

Isn't it weird that all of the HTML files are called `index.html`? <span class="major-key">When a folder
contains a file named `index.html`, that is the default
page that will be shown when you don't specify a file name.</span>

We could have built it so that the iOS track was contained in a file called `ios.html`, and then you could view the page by navigating to `learn.devfe.st/ios.html`—but it's cleaner to organize everything so that you only have to navigate to `learn.devfe.st/ios/`, which will automatically display the file at `learn.devfe.st/ios/index.html`.

The directory
structure looks something like this:

    learn.devfe.st/
      - index.html
      - beginner-dev/
        - index.html
      - data-science/
        - index.html
      - game-dev/
        - index.html
      - ios/
        - index.html
      - product/
        - index.html
      - web-dev/
        - index.html

In reality, there are other files apart from the HTML, so this is a little
simplified. Still, this should help clarify the structure.

<a id="inspector"></a>
### How do we know what's going on in the browser?

We're almost ready to build out our own content! But first, we have an
important tool to talk about.

If something's broken on your site, how do you
know what's happening? Or, maybe more interesting, if you see something
awesome on another website, how do you find out why it looks the
way it does?

Fortunately, this problem has already been solved beyond our wildest
dreams by very smart people! You can **inspect element** by
right-clicking in Chrome, Safari, or Firefox. (In Safari, you might have
to [enable this
manually](https://developer.apple.com/library/iad/documentation/AppleApplications/Conceptual/Safari_Developer_Guide/GettingStarted/GettingStarted.html)).

You can also view the **source code** in
`Tools > Web Developer > Source Code` in Firefox,
`View > Developer > View Source` in Chrome, and
`Develop > Show Page Source` in Safari.

Try viewing the source for this page now! You'll see some things that
look familiar, and some things that might look a little bizarre. It's
great practice to do this whenever you come across a website you really
like and want to see what's going on under the hood.

<span class="major-key">If there's something you don't understand,
Google it. Always. Every time.</span> Most of the learning we do as
developers happens while we're on the job, or building something on our
own, not from tutorials like this. Don't be afraid to explore and learn
something new.

Let's review some of the language we covered in this lesson. I know this
might seem a little silly, but there's actually a great reason to focus
on vocabulary, and it's not because I want to treat this like a middle
school English class.

<span class="major-key">It is really important to be able to hold a
technical conversation.</span> This is something I wish I'd learned
earlier on in my life as a programmer! You'll be able to communicate
much more easily with other developers if you understand these words and
know when it's appropriate to use them.

<a id="terms-html"></a>
### Terms you should know

HTML
:   Stands for HyperText Markup Language. A standard developed in 1991
    by Tim Berners-Lee.

element
:   A component of an HTML page. Every HTML page is made up of elements.

tag
:   The code that opens and closes HTML elements. `<p>` is
    an **opening tag**;`</p>` is a **closing tag**.

headers
:   Also known as **headings**, although that terminology is
    getting outdated. Generally speaking, they describe the topic of
    a section. In decreasing order of priority, they go from
    `<h1>` to `<h6>`.

anchor tags
:   More commonly known as links, represented by
    `<a href="http://some-link.com">`.

attribute
:   A property of an HTML element, like the `href` in a
    link or the `src` in an image.

nesting
:   HTML elements can be **nested** inside one another.

parent/child
:   A **child** element is nested inside its **parent**.

comment
:   Helps to clarify your code. Only visible in the **source code**. In
    HTML, `<!--` opens a comment and `-->`
    closes a comment. Comments are formatted differently in
    every language.

root directory
:   The top folder in a file system.

source code
:   Raw code written by a programmer. HTML source code is viewable using
    the developer tools in your browser.

inspect element
:   You can **inspect element** using your browser to view the
    properties of a specific HTML element.

<a id="project-html"></a>
### A short project

Now it's time to apply what you've learned! Let's build something fun.

#### Getting started

Create a folder at the same level as your `Documents`
folder. It will be your working directory for the remainder of this
tutorial.

Open up [Sublime Text](http://sublimetext.com). You should have
downloaded this already, but if not, do so now!

In Sublime Text, create a new file called `index.html` and
save it inside your working directory.

#### Working on the file

You can view the HTML file in your browser by right-clicking and
choosing "Open with...", then choosing your browser.

Whenever you want to update your file, make sure you save the file!
Saving is very important, not only to make sure your work doesn't
disappear, but also because your browser will only display the most
recently saved version.

#### Checklist

-   A header with your name in it.
-   A picture of you. Or of your favorite pokémon. Or your least
    favorite rapper.
-   A paragraph describing yourself. Or your favorite pokémon, or least
    favorite rapper.
-   At least three links to other websites.

___________
<a href="#top" class="top" id="css">Top</a>
## Level 2: CSS

Hopefully, you've recently finished building yourself a complete page in
HTML. “But wait,” you say. “This isn't what real websites look like.
This is what garbage websites look like!”

Even if your HTML looks perfect, it's not enough on its own. Thankfully,
we have CSS: a tool to help our websites not look like garbage.

<a id="intro-css"></a>
### What is CSS? What does it look like?

<span class="major-key">CSS modifies properties of HTML elements.</span>
Here's what it looks like:

    p {
        font-size: 20px;
    }

That snippet of CSS will set the font size of all paragraphs on an HTML
page to 20 pixels.

More generally, a CSS **rule** is formatted like this:

    [selector] {
        [property]: [value];
        [property]: [value];
        [any arbitrary number of property/value pairs]
    }

CSS has a strange learning curve, because almost none of the knowledge
is conceptual; instead, learning CSS comes down to getting familiar with
a lot of different properties one at a time, and trying a lot of
different solutions when problems come up. Once again, Google will be
your friend!


In order to write CSS, we have to get familiar with **selectors**: the
strings that determine which elements your CSS rules are applied to.

    [selector] {
        [property/value pairs]
    }

<a id="selectors"></a>
### Selectors

There are a couple different ways we can specify HTML elements using
selectors. Let's dive in!

#### Element type

In the first example on this page, the selector was just one character
long: `p`. That selector means that the CSS rule applies
to all `<p>`'s on the page.

We can do the same thing with any HTML element: `a`,
`h1`, `body`, you name it. However, it's
important to note that <span class="major-key">many CSS rules will apply
not only to the selected elements, but also to their children.</span>
For example, check out the following rule:

    body {
        color: red; /* the "color" rule sets text color */
    }

This will make all of your website's text red, because all of the page's
content is nested inside the `body`.

#### Classes

What if you wanted a CSS rule to only apply to certain paragraphs?
That's what **classes** are for! Check out this snippet of HTML and CSS:

    <body>
        <p>This is a normal paragraph.</p>
        <p class="special">This paragraph is special, mmkay?</p>
    </body>
&nbsp;

    p {
        color: red;
    }

    .special {
        font-size: 36px;
    }

A class is just another attribute of HTML elements. In order to use a
class as a CSS selector, all you need to do is add a `.`
to the beginning of the class name in your CSS.

In the example above, both paragraphs will be red, because the
`color: red` rule applies to every `<p>`
element. But only the second paragraph will have a larger-than-normal
font-size.

You can apply any class to as many HTML elements as you want. Let's look
at another example:

    <body>
        <p>I'm a normal paragraph.</p>
        <p class="small">I am so small.</p>
        <p class="small">I am so small.</p>
        <p class="small">I am so small.</p>
    </body>
&nbsp;

    p {
        color: red;
    }

    .small {
        color: blue;
        font-size: 8px;
    }

Only the first paragraph will have a normal font-size; the last three
will be super small.

But what about their color? The last three paragraphs have two different
rules that affect their color: all `<p>`'s have
`color: red`, but all elements with the
`small` class have `color: blue`. Will this
break something?

Nope—the last three paragraphs are all blue! CSS is smarter than you
might think, and it knows that the `.small` rule is more
specific than the rule that applies to all paragraphs. Therefore, if
there are any conflicts for a specific HTML element, CSS follows the
most specific rule that applies to it.

#### Combining selectors

What if you wanted a rule to apply to multiple selectors? CSS makes that
easy, too!

    <body>
        <h1>Pokemon are sick</h1>
        <p class="big-red">Charizard</p>
        <p class="big-blue">Blastoise</p>
        <p class="big-green">Venusaur</p>
        <p>Digimon is for scrubs</p>
    </body>
&nbsp;

    .big-red {
        color: red;
    }

    .big-blue {
        color: blue;
    }

    .big-green {
        color: green;
    }

    h1, .big-red, .big-blue, .big-green {
        font-size: 72px;
    }

You can use commas to combine selectors (both HTML element selectors
like `h1` and class selectors like
`big-red`). In this example, everything except the last
paragraph has a font-size of `72px`.


Now, we're ready to talk about the different kinds of properties you can
set using CSS! There is a truly enormous number of them, so let's focus
on three different categories: text, colors, and positioning.

<a id="text"></a>
### How can I customize text with CSS?

Typography can be one of the most fun parts of building a website, if
you are a nerd like me. Let's go through some relevant CSS properties to
help make your text look excellent!

#### font-size

Sets the size of the text. There are several valid **units** for
properties like this, but let's stick to `px`, because
it's consistent and easy to use.

<span class="font-size-1">font-size: 10px;</span>

<span class="font-size-2">font-size: 18px;</span>

<span class="font-size-3">font-size: 32px;</span>

Generally, the most readable size for text is around 18 or 20
`px`, but it will depend on the font and the context. Note
that a little change goes a long way when it comes to pixels!

#### line-height

This attribute will control the **line-height** of your text. Again,
we'll use `px` as units. To help show this visually, I've
changed the `background-color` of these next paragraphs,
which we'll talk about soon!

&nbsp;&nbsp;&nbsp;&nbsp;

line-height: 16px;
<span class="line-height-1">If your line-height is the same value as your font-size, it still might
look cramped. If your line-height is the same value as your font-size, it still might
look cramped. If your line-height is the same value as your font-size, it still might
look cramped. If your line-height is the same value as your font-size, it still might
look cramped. If your line-height is the same value as your font-size, it still might
look cramped.</span>

line-height: 32px;
<span class="line-height-2">Because double-spacing isn't just for making your essays hit ten pages!
This can look awkward, too, though, so be careful. Because double-spacing isn't just for making your essays hit ten pages!
This can look awkward, too, though, so be careful. Because double-spacing isn't just for making your essays hit ten pages!
This can look awkward, too, though, so be careful.</span>

&nbsp;&nbsp;&nbsp;&nbsp;

Some people believe that the ideal line-height is (font-size × 1.618),
which is the [golden
ratio](https://en.wikipedia.org/wiki/Golden_ratio){.ALMIGHTY-GOLDEN-RATIO}.

#### font-weight

Font-weight can be a finicky attribute, because it depends on the font
you're using. The two most common values are `400` and
`700` (no units), which translate to "normal" and "bold".

<span class="font-weight-1">font-weight: 400;</span>

<span class="font-weight-2">font-weight: 700;</span>

#### font-style

Font-style should be used as nothing more than an on/off switch for
italics. Relevant values are `italic` and
`normal`.

*font-style: italic;*

font-style: normal (default value);

#### font-family

Font-family might be the most important attribute, because it lets use
choose our actual font! There are several built-in fonts that will work
in any browser (of which Times New Roman is the most infamous), but we
can do better than that.

<span class="font-family-1">font-family: Times New Roman</span>

<span class="font-family-2">font-family: Helvetica</span>

<span class="font-family-3">font-family: Lato</span>

Lato isn't a built-in font, but I can use it thanks to [Google
Fonts](https://google.com/fonts). Google Fonts gives you free access to
thousands of different fonts, and it's extremely useful. It's easy to
use: once you select a font and some weights, all you have to do is
insert an HTML snippet—which they provide for you—into your website's
`head`! Here's the one I used to get that snippet:

    <link href='https://fonts.googleapis.com/css?family=Lato:400' rel='stylesheet' type='text/css'>

That snippet of HTML is all I need to use Lato wherever I want on the website.


Now that we have some typesetting skills, let's take a look at colors!
Nothing in life is black and white, so your website shouldn't be either.

<a id="colors"></a>
### How do colors work in CSS?

While it's possible to make a paragraph red using
`color: red`, you will quickly find that that won't offer
you a whole lot of creativity. CSS allows you to be much more specific
than that!

#### RGB

There are several options for syntax, but a good alternative is **RGB**,
where you specify a value between 0 and 255 for red, green, and blue.

<span class="color-1">color: rgb(0, 0, 0);</span>

<span class="color-2">color: rgb(0, 0, 255);</span>

<span class="color-3">color: rgb(42, 136, 252);</span>

Remember: `rgb(0, 0, 0)` is black and
`rgb(255, 255, 255)` is white.

#### Hex

You should also be familiar with **hexadecimal notation**, or more
simply, **hex values** (or **hex codes**). Here's what it looks like:

<span class="color-1">color: \#000000;</span>

<span class="color-2">color: \#0000FF;</span>

<span class="color-3">color: \#2A88FC;</span>

Hex codes work the same way as RGB, where red, green, and blue each get
a value from 0 to 255. However, hex uses just two characters for each:
they're numbers in [base 16](https://en.wikipedia.org/wiki/Hexadecimal).
The second example above, `#0000FF`, translates to
`rgb(0, 0, 255)`. The first two numbers,
`00`, translate to a red value of 0; the second two
numbers, `00`, translate to a green value of 0; and the
final two numbers, `FF`, translate to a blue value of 255.

#### In context

Let's look at some examples of using colors in context.

-   Setting text color

    We've done this before! You can set text color just by using the
    `color` attribute.

        .white-text {
            color: rgb(255, 255, 255);
        }

-   Setting a background color

    Every element has a default background color of white, but it's easy
    to change. You can change the background of your whole website just
    by changing the `background-color` of the body.

        body {
            /* This will make your whole website neon green */
            /* Not a great idea */
            background-color: rgb(0, 255, 0);
        }


We have one more topic of CSS attributes to cover: positioning.
Positioning things using CSS can be frustrating, but you'll learn
quickly! And by that I mean you'll quickly learn that CSS is completely
unusable and broken forever. Welcome to the party.

<a id="position"></a>
### How do I position elements on a page?

CSS gives us many tools to solve the problem of placing something on a
page. Often, there are multiple solutions to the same problem.

#### Position

**Position** is an important CSS attribute to understand. It only has a
few possible values, but they are all very powerful. Let's look at the
most relevant ones:

1.  `position: fixed`

    This is the easiest position to work with. A fixed element stays in
    the same visual spot on your browser no matter what. Notice how the
    hamburger menu on the top left stays in the same place no matter
    where you're scrolling. That element is
    `position: fixed`!

    To use this, you also need to specify one or more of the following
    attributes: `top`, `bottom`,
    `left`, `right`. Here's an example of a
    button that will stay in the bottom right of the page:

        .button {
            position: fixed;
            /* the bottom of the button will always be
                20px from the bottom of the window */
            bottom: 20px;
            /* the right edge of the button will always be
                20px from the right side of the window */
            right: 20px;
        }

2.  `position: absolute`

    This works a lot like `position: fixed`, except that
    instead of fixing an element to the window, it fixes an element to
    its parent, as long as the parent is
    `position: relative`. Once again, you'll generally
    need to also specify one or more of `top`,
    `bottom`, `left`, or
    `right`.

3.  `position: relative`

    Relatively positioned elements generally behave as you'd expect
    them to. When you specify any position on a relatively-positioned
    element (`left`, `right`, etc.),
    everything else is positioned by ignoring the changes to the
    relatively-positioned element. In other words,
    `position: relative` is a good way to change the
    position of only one element.

Position is a difficult attribute to visualize. I'd recommend checking
out the
[CSS-Tricks](https://css-tricks.com/almanac/properties/p/position/) and
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/position)
articles on position to get a better picture. In general, <span
class="major-key">[CSS-Tricks](https://css-tricks.com) and
[MDN](https://developer.mozilla.org/en-US/) are excellent references for
anything CSS-related</span>. I always learn something when I read an
article from them.

#### Width and Height

You can specify both the width and height of HTML elements using these
attributes. Use either `px` or `%` as units.
<span class="major-key">When using `%`, bear in mind that
the percentage is computed as the percentage of the parent element's
width or height</span>.

    <body>
        <div class="container">
            <p class="text">I am so tall</p>
        </div>
    </body>

&nbsp;

    .container {
        height: 800px;
    }

    .text {
        /* ends up being 800px, because its parent's height is 800px */
        height: 100%;
    }

#### Text-Align

This rule aligns text, like Microsoft Word or Google Docs. Possible
values include `left`, `center`,
`right`, and `justify`. Don't be a dingus,
though—you should only ever use `left` and
`center`.

    <body>
        <div class="text-container">
            <p class="text">The Middle - Jimmy Eat World</p>
        </div>
    </body>

&nbsp;

    .text-container {
        text-align: center;
    }

In the above example, note that we must set the paragraph's parent to
`text-align: center`, not the paragraph itself!
`Text-align` rules apply only to an element's children.

#### Padding and Margin

There's one more positioning trick we should be familiar with: using
**padding** and **margin**. Units should be `px`.

Padding adds space inside an element, and margin adds space around an
element. Here's a helpful visualization:

<div class="image-wrapper">

<img src="https://css-tricks.com/wp-content/csstricks-uploads/firebox.png">

</div>

That model shows an HTML element with a `width` of
`267px` and a `height` of
`24px`. It has `6px` of
`padding` on every side, no border or margin, and it has
`top: 156px`. You can actually see this box model for any
HTML element by right-clicking the element and choosing
`inspect element`!

You can put padding on specific sides of an element by using
`padding-right`, `padding-top`,
`padding-left`, and `padding-bottom`; same
with margin. If the rule doesn't include a direction, like
`margin: 5px;`, then it will apply `5px` of
margin to every side of the element.


Now that we've learned some useful CSS rules, we'll learn how to
integrate a CSS file with our HTML!

<a id="linking-css"></a>
### How do I put CSS in my HTML file?

Just like HTML, you can write all of your CSS in one file, as long as
you end the filename in `.css`. Create a folder called “css”
and put the file there. Then, in your HTML file, link to the CSS file in
the `head`, using the following syntax:

    <head>
        <title>How Website</title>
        <!-- The href for the CSS will be different depending on
            whether you put the CSS file in a new directory, which is
            what I've done here. -->
        <link rel="stylesheet" type="text/css" href="css/style.css">
    </head>

A consequence of this is that you can have one CSS file for multiple
HTML files. Here's what your directory structure should look like now:

    website/
      - css/
        - style.css
      - index.html


If you want to use Google Fonts (and you should!), <span
class="major-key">you must import the font before
importing the CSS file in your `head`</span>, like so:

    <head>
        <title>Kylo Ren's Personal Blog</title>
        <link href='https://fonts.googleapis.com/css?family=Lato:400,700,900,400italic' rel='stylesheet' type='text/css'>
        <link rel="stylesheet" type="text/css" href="/css/style.css">
    </head>


Wow, we covered a lot of content! Now let's learn some words.

<a id="terms-css"></a>
### CSS terms

CSS
:   Short for Cascading Style Sheets. Nobody knows that, though, so
    don't bother remembering it.

rule
:   A complete snippet of CSS: a selector and a property-value pair.

selector
:   A string that specifies HTML elements.

class
:   A special HTML attribute that makes it easy to select a group of
    elements with CSS.

unit
:   Most CSS values require units, like `px` or
    `%`.

line-height
:   The vertical space taken up by each line of text in an HTML element.

RGB
:   A format for describing colors: `rgb(0, 0, 0)`. Each
    value can range from 0 to 255.

Hex values/hex codes
:   A more compact color format: `#00FF00`. Works the same
    way as RGB: the first two characters correspond to red, the next two
    correspond to blue, the last two correspond to green. Each pair of
    characters can range from `00` to `FF`.

Position
:   A property that determines how an element's position is calculated.
    You should be familiar with the values `fixed`,
    `relative`, and `absolute`.

Padding
:   Spacing between an element's content and its border.

Margin
:   Space outside of an element's border.


<a id="project-css"></a>
### Explore the wonderful world of CSS

OK, let's goof around a little bit! I always find that when designing
websites, and when using CSS in general, I get the best results when I
try a lot of different things. So that's what we'll do now!

For this mini-project, we'll be reusing the HTML page we created at the
end of the last lesson.

#### Getting started

Create a new folder called “css” inside the same folder that contains
your HTML file, then create a new file inside “css”. You can call it
`style.css` if you're boring like me.

In your HTML file, link to the new CSS file in the `head`,
using the [snippet from above](#linking-css). Add a simple rule to your CSS,
like making all the text enormous, then save everything and refresh. If
you can't see the change visually, be extra careful about your directory
structure and make sure the file name is spelled right in the HTML
(case-sensitive!).

Once everything is linked properly, let's get started!

#### Tasks

These are all open-ended, so exploration is encouraged! If you get bored
with something, move onto the next thing. The only goal here is to try
enough things that you end up with something good and unexpected.

Use [Google Fonts](https://google.com/fonts) to try out a couple of
different font options for your website.

-   For each font, try a couple of different sizes and weights. Also,
    try different combinations of header font-size and text font-size.

Once you have a couple of different options for fonts, try at least four
different color schemes, including background colors. Here are some
suggestions:

1.  Use 4 different colors on your site
2.  Use only 2. This is actually really hard!
3.  Try a dark theme
4.  Try using the color scheme of your favorite-designed website.
    [BuzzFeed](https://buzzfeed.com) and [Lyft](https://lyft.com) are
    two great places to start.

Try out at least 3 different layouts. You can follow these suggestions,
or get creative!

1.  Try putting your links at the bottom of the page.
2.  Try putting everything in the middle of the page.
3.  Try filling the page with your image, using [this
    guide](https://css-tricks.com/perfect-full-page-background-image/).

Once you've finished trying everything, see if you can decide on two or
three different themes for your site. Then, create a separate CSS file
for each theme: that way, switching between themes on your HTML page
will be as easy as changing the `link` snippet in the
HTML!

___________
<a href="#top" class="top" id="js">Top</a>
## Level 3: JavaScript

Believe it or not, we already have most of the tools we need to make a
fully-functioning website. However, HTML and CSS impose some frustrating
restrictions on web development that get completely blown away when you
have some familiarity with JavaScript.

It would be impossible to offer a complete course in JavaScript on one
page of an introductory web development course, so let's take a little
bit of a different approach to this. Instead of learning JavaScript
concepts from the ground up, we'll learn how to do some cool things with
an easy-to-use JavaScript **library** called **jQuery**.

We'll cover a lot of ground in a short amount of time, and we'll come
out on the other side of this lesson with some really, really cool
tricks up our sleeves. Onwards and upwards!

<a id="console"></a>
### JavaScript in the Console

Let's start by opening up the **console**! To do this, inspect element
anywhere on this page, then choose "console" from the tabs at the top of
the inspector. Inside the console, type
`console.log("Hello website!");`, and press enter.

The console is like a little JavaScript sandbox. When you write
JavaScript statements in the console, it gets interpreted just like any
JavaScript that might have already been included on the website. That
means <span class="major-key">the console is a great place to experiment
with JavaScript</span>! Bear in mind that anything you do in the console
only affects your current session in your browser. So, if you mess
anything up super bad, you can always just refresh.

You can open up the console on any website you visit! Because any
JavaScript errors also get reported to the console, there might already
be a lot of garbage inside the console, depending on the site. No matter
what, though, you'll always be able to type things into the console and
play around with the HTML on the website.

You can also use `console.log` statements in JavaScript
files. It'll print whatever you put inside the parentheses to the
console.

One last thing: you should run all of the JS snippets from this lesson
in your console. If you want to live life to the fullest, try modifying
each of the snippets a little bit after running them to make sure you
understand what's happening and see what works.

<a id="variables"></a>
### JavaScript variables

In JavaScript, we need to be familiar with the concept of a
**variable**. Variables provide a way for us to store values.

    var myFavoriteRapper = "Drake";
    console.log("My favorite rapper is " + myFavoriteRapper);

This is a short snippet of JavaScript, but there's a lot to talk about!
Let's start by breaking the first line into five separate components.

1.  The **keyword** `var` indicates that we're
    **declaring** a variable.
2.  The name `myFavoriteRapper` is how we'll refer to this
    variable in the code after this line in our JavaScript file.
3.  The `=` sign is the assignment operator in JavaScript.
    It stores whatever value is on the right side of the operator into
    the variable on the left side.
4.  `"Drake"` is the value being stored into the variable.
5.  The semicolon, `;`, indicates that the **statement**
    is finished. Every JavaScript statement must end in a semicolon. For
    now, we can think of a statement as being equivalent to a line
    of code.

The second line of code in that snippet should look familiar. We're just
logging something to the console, but notice what's inside the
parentheses:
`"My favorite rapper is " + myFavoriteRapper`. This
expression gets **evaluated** to the string "My favorite rapper is
Drake", because you can add strings together with a + sign in
JavaScript. `myFavoriteRapper` contains the string
`"Drake"`, so JavaScript puts the two strings together; it
doesn't care that one of the strings is stored in a variable.

Now let's look at an extended version of this snippet.

    var myFavoriteRapper = "Drake";
    console.log("My favorite rapper is " + myFavoriteRapper);
    myFavoriteRapper = "Kendrick";
    console.log("Just kidding. It's " + myFavoriteRapper + ".");

Now that we've already declared the `myFavoriteRapper`
variable, we don't use the `var` keyword anymore when we
want to change the variable's value. Now, when we use the variable in
the last line, JavaScript evaluates it to the value to which it was most
recently set: `"Kendrick"`.

If you ran that snippet in the console, or put it in a JavaScript file,
you would get the following output:

    My favorite rapper is Drake
    Just kidding. It's Kendrick.

<a id="arrays"></a>
### Grouping values with arrays

Before we take a look at all the tricks we can do with jQuery, we need
to cover one more JavaScript fundamental: the **array**. Arrays are
useful for storing groups of values, where it would be unwieldy to have
a variable for every single one.

    var numbers = [4, 8, 15, 16, 23, 42];
    console.log(numbers[1]);

In this example, `numbers` is a variable that stores an
array that contains six values. We can access these values with the
syntax `arrayName[index]`. So, the expression
`numbers[1]` will evaluate to the whatever's stored at
position 1 in in `numbers`.

However, the thing that's stored at position 1 in
`numbers` is actually `8`! That's because
arrays are **zero-indexed** in JavaScript, meaning that the indices
start at 0. So, to get the first element in `numbers`, we
would need to write `numbers[0]`.

--------------

Let's take a break for a second! We're going through these concepts
really quickly. I'd recommend going back and rereading the JavaScript
we've covered up until now, making sure you understand everything that's
going on in the snippets.

If you don't understand everything completely, please read Chapters
[1](http://eloquentjavascript.net/01_values.html) and
[2](http://eloquentjavascript.net/02_program_structure.html) of [Eloquent
JavaScript](http://eloquentjavascript.net/). It offers a much more complete background to what we're
doing now.

If you do understand all the snippets, read Chapters 1 and 2 of Eloquent
JS anyway! Read more if you have the time. Trust me when I say that it
will serve you well in the long run.

Also, it's OK if this stuff feels hard. JavaScript is such a vast and
deep topic that it's impossible to get the hang of it quickly. Remember:
if you meet anyone who says they're a JavaScript expert, they are either
very very experienced or wrong.

Once you feel like you're up to speed, we'll learn how to make it work
with HTML!

<a id="linking-js"></a>
### Putting JavaScript on your website

Inserting JavaScript into a website is pretty similar to linking to a
CSS file. Use a `script` element to include your file
right at the bottom of your `body`:

    <!DOCTYPE html>
    <html>
        <head>
            <!-- All your head attributes -->
        </head>
        <body>
            <!-- Content goes here -->
            <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
            <script src="/js/index.js"></script>
        </body>
    </html>

Note that, based on the `src` attribute of the
`script`, `index.js` is inside a folder.
This follows the same pattern we established in the CSS lesson: create a
folder called `js` and put it at the same level as your
`index.html`, so that any JavaScript files will live
inside that new folder. Your files should now look like this:

    website/
      - css/
        - style.css
      - js/
        - index.js
      - index.html

<a id="jquery"></a>
### jQuery is your friend

jQuery makes JavaScript easier to use. With jQuery, selecting all the
paragraphs on a page is as easy as `$('p')`, where the
pure-JS analogue would look like
`document.getAllElementsByTagName('p')`. Anytime you see
or use a `$` in JavaScript, that means you're using some
features from jQuery.

Before we go any further, let's draw some hard lines about what jQuery
is and how to use it.

#### What jQuery Actually Is

In the introduction, I said that jQuery was a JavaScript library, but I
didn't explain any further. What that means is that it's a collection of
pre-written JavaScript utilities that abstract away a lot of the
headaches caused by doing things in JS that feel like they should be
easy, but end up being complex and annoying. jQuery isn't another
programming language, even though it can feel like one sometimes. That
means that you can use jQuery in normal JavaScript files, as long as you
import the jQuery library on your website.

#### Importing jQuery

There are a couple of ways to put jQuery on your website, but the one
I'd recommend is by letting Google host it. This is actually the same
way Google Fonts works: you just link to the content from Google before
you link to your own code. Again, the snippet goes at the bottom of the
`body`:

    <body>
        <!-- Content goes here -->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
        <script src="/js/index.js"></script>
    </body>

OK! We're ready to do some wild things using jQuery and JavaScript.

<a id="selectors-jquery"></a>
### Using jQuery selectors

As I mentioned before, selecting all the paragraphs on the page is as
easy as `$('p')` when you use jQuery. Selecting things in
jQuery works a lot like CSS: you can select based on class names or tag
names, and you can combine selectors with commas.

    $('a')
    $('.major-key')
    $('h1, h2, h3, h4')

Each of these selections returns an array of HTML elements—just like
arrays can contain numbers or strings, they can also contain more
complex objects like HTML elements. For example,
`$('a')[0]` would give you the first link on the page. Try
this in the console now!

This means that jQuery makes it really easy for us to manipulate a lot
of HTML elements all at once. For example, we can change the content of
HTML elements really easily. Try running the following line of code in
your console:

    $('code').html('lol');

(Unfortunately, there is no concept of an “undo” button in the console.
Remember how I said you'll sometimes have to refresh to get things back
to their original state?)

There are other, less destructive things you can do with HTML in jQuery.
Let's take a quick look now:

    // Returns content of first HTML element that matches the selector
    $('code').html();

    // Inserts HTML snippet at end of element (inside the element)
    $('h3').append(' <a href="https://www.youtube.com/watch?v=iZJXvjeWlVA">:O</a>');

    // Inserts HTML snippet after element
    $('h3').after('<p>Time to learn!</p>');

The opportunities are endless! The world is your oyster!

<a id="events"></a>
### <span class="major-key">Handling events with jQuery is a major key</span>

What we've seen so far makes it easy to do some silly things. But what
if we could manipulate HTML elements depending on what the user does?
Suddenly, we'd have a lot more power. That's what **events** are for!
Let's take a look at an example.

    $('code').on('click', function() {
      $(this).html('wow lol');
    });

This is a snippet that changes the content of every
`code` element when you click on it. Copy and
paste it into the console to see what the effect is! Let's go through it
carefully to understand what's really going on.

    // For everything that matches this selector,   when you click it,   do this thing:
    $('.inline-code')·······························.on('click',········ function() {

    // Change only the clicked element's HTML content to   "wow lol".
      $(this).html········································ ('wow lol');

    }); // (closing parens and braces as necessary)

Along with `click` events, there are some other events
that are useful to know when building things with jQuery:

-   `dblclick`: double-click on an element
-   `mouseover`: user's mouse moves on top of an element
-   `mouseout`: user's mouse leaves an element
-   `mousemove`: user moves their mouse
-   `keydown`: user presses a key on their keyboard (to
    trigger actions based on which key they pressed, check out
    [these](http://eloquentjavascript.net/14_event.html#c_HHTiM1P8JU)
    [references](http://unixpapa.com/js/testkey.html)!)
-   `scroll`: user scrolls (if you're viewing this on
    Chrome on a desktop, there's a special effect on the page that
    uses this!)

<a id="jquery-css"></a>
### Manipulating CSS with jQuery

One of the most useful things you can do with jQuery is changing CSS
based on certain events. Just like we can manipulate HTML content with
`html`, we can change all kinds of CSS using
`css`.

    $('p').on('click', function() {
      $(this).css({
        "color": "#42cbad",
        "font-weight": "700",
        "line-height": "40px",
      });
    });

Note that each property-value pair is in quotes, and goes inside curly
braces (`{}`). Also, each pair has a comma after it,
though the comma on the last pair is optional.

One big disadvantage of this approach is that you can't bring any
clicked element back to its original state. What if we wanted to just
switch between styles on every click? There are some ways to do that
with just JavaScript, but the most elegant solution involves CSS, too!

    /* I included this in my CSS so that you could run the snippet below! */
    .extra-cool-text {
      color: #42cbad;
      font-weight: 700;
      line-height: 40px;
    }

    $('p').on('click', function() {
      $(this).toggleClass('extra-cool-text');
    });

Now, instead of manipulating CSS attributes directly with JavaScript,
we're just changing whether each element has a class applied to it.
`toggleClass` is extremely useful.

<a id="animation"></a>
### Animating things with jQuery

One of the most fun, and equally useless, things you can do with jQuery
is animation! jQuery makes this incredibly easy. The code looks a lot
like changing CSS, but you must also provide the number of milliseconds
you want the animation to take.

    $('h3').on('mouseover', function() {
      $(this).animate({
        "letter-spacing": "10px",
        "font-size": "40px"
      }, 1000);
    });

Tears of joy. You can also chain animations together to specify the order in which
the animations happen, like this:

    $('h3').on('mouseover', function() {
      $(this).animate({ "font-size" : "40px" }, 400)
      .animate({ "letter-spacing" : "10px" }, 1000);
    });

Note that I'm formatting the code a little differently in this snippet:
I'm fitting more stuff on one line. That's because JavaScript doesn't
care about whitespace or whether or not you have newlines (i.e. press
return) between different statements. When you chain animations
together, you might find it easier to read visually when you put each
animation on its own line.

You can also give the animation something called a **callback**
function: some code that will run after the animation finishes. This is
optional, and comes after the animation length, separated by a comma,
like this:

    // Run this in the console, then click me
    $('code').on('click', function() {
      $(this).animate({
        "height" : "0px",
        "padding": "0px"
      }, 400, function() {
        $(this).html("");
        alert("goodbye world"); // like console.log() but better
      })
    });

You can put anything that's valid JavaScript inside of that callback
function.

<a id="document-ready"></a>
### `$(document).ready`

Before I send you off into the real world of jQuery silliness, I have
one last piece of advice, and it's important.

You can't safely manipulate any HTML until all of the content has
actually been loaded. You'll experience some strange and frustrating
bugs if you try to do so. But how do we know when the page is safe for
JavaScript? It seems like a difficult problem.

    $(document).ready(function() {
      ...
      // All JS code goes here!
      ...
    });

Well, it is indeed a difficult problem, but it's not one you have to
solve! This is another great feature of jQuery. As long as you put all
of your code inside those beginning and ending lines, you'll never
experience the pain of those problems.

Cool! We've put together a pretty hilarious toolbox of effects with
jQuery. Let's review some language from this lesson, then dive into a
mini-project.

<a id="terms-js"></a>
### JS terms you should know

JavaScript
:   A programming language for the web, created in May 1995 in 10 days
    by Brendan Eich.

JavaScript library
:   A collection of prewritten utilities in JavaScript.

jQuery
:   An all-purpose JavaScript library.

console
:   The browser's interface between you and JavaScript.

keyword
:   A reserved word in JavaScript (or any other programming language!).
    Examples of keywords would include `var` or
    `function`.

variable
:   A container that stores a value. Every variable has a name, assigned
    by the programmer.

declaring a variable
:   Creating a variable for the first time. Requires the
    `var` keyword.

statement
:   A complete JavaScript operation, analogous to a sentence.

evaluate
:   The process by which JavaScript determines an expression's value.

array
:   A structure that contains 0 or more values.

zero-indexed
:   Describes the convention that states that the first element in an
    array has an index of 0.

event
:   Any of several different user actions performed in the browser, e.g.
    `click`, `mouseover`,
    `mousemove`.

callback
:   A function that gets executed once the current function
    has finished.

<a id="project-js"></a>
### Very Serious Assignment

#### Getting started

To get started, make sure your directory structure looks like what we
covered [above](#linking), and make sure your HTML file links to both
jQuery and to your own JavaScript file.

#### Your mission

Let's do some fun stuff with jQuery! Like all our assignments have been,
this one will be pretty open-ended: all I ask is that you spend at least
45 minutes goofing around with the effects we talked about. If you want
some inspiration, here are some ideas!

-   Make some links titled "Facebook", "Twitter", "LinkedIn"—normal
    social media outlets or whatever. When the user clicks on the link,
    though, instead of taking them to Facebook or Twitter or whatever
    garbage company, just change the link's HTML content to be a
    description of what the product does.
-   Design your website so that when everything loads at first, all the
    user sees is white. But over the course of one minute, your content
    gradually fades in, ever so slowly.
-   Make a "dark theme" button that toggles your website between light
    and dark themes. See how I used that word "toggle"?
-   Make a "sith mode" button that toggles your website between light
    and dark themes, where the dark theme also replaces all your images
    with pictures of Kylo Ren looking sad. (This one is a little harder,
    but I put it here anyway because I really want to see it in
    real life.)

------------------------------
<a href="#top" class="top" id="git">Top</a>
## Level 4: Git

From an early age, it is instilled into us that we must always
`command-S` every chance we get, so that we don't lose
precious work. But what if we want to work on two versions of a project
simultaneously? Or we're working with 4 other people, all on the same
file? Or 100 people? The need for **version control** is great, and Git
is our savior.

A long time ago, I told you to set up
[git](https://help.github.com/articles/set-up-git/) and register for
[GitHub](https://github.com), so if you haven't already, do so now!
You'll need them to get through the lesson; instead of going through
content and then doing a mini-project at the end, this will be a little
more interactive.

Mac users, open your terminals; Windows users, open Command Prompt.
Let's get to it!

<a id="terminal"></a>
### Navigation in the terminal

Before we start looking at Git, let's make sure we have enough knowledge
about our terminal to be able to move around folders and files.

#### `pwd`

If you're a Mac user, in your terminal, type `pwd` and
press enter. This is the first of several **commands** we'll cover, and
it shows you exactly where you are in your terminal. That's why the
command is called `pwd`: it stands for Print Working
Directory.

Windows users won't have to worry about `pwd`, because
Command Prompt will always show your complete location.

<span class="major-key">If you're ever confused or want to learn more
about a specific command, just run `man [command]` on
Macs, or `HELP [command]` on Windows</span>. For example,
you can type `man ls` and you'll see more information than
you'd ever want to know about `ls`! On Macs, you'll have
to press `q` in order to exit the manual view.

#### `ls`

Once you've figured out what directory you're in inside your terminal,
run `ls` (`dir` on Windows). You'll see a
list of all the files and folders inside your current directory.

#### `cd`

Now that you can see all your files and folders, we'll talk about
navigating between folders. If you've just run `ls` or
`dir`, you'll be able to see a bunch of folders, like
Documents and Downloads. Try running `cd Documents` now.
This will bring you into the Documents folder, and you can
`ls` or `dir` to see how poorly organized
your Documents folder is.

To get back to where you were, type `cd ..`:
`..` always stands for the parent directory, and
`.` always stands for the current directory.

OK, now we're ready to get started with git!

<a id="intro-git"></a>
### Creating and cloning your first repo

First, login to GitHub and create a new **repository**. Name the
repository \[your-username\].github.io, make it public, and check the box
that says “Initialize this repository with a README”.

Once you've created the repository (**repo** for short), GitHub will
take you to the repo's freshly created page. Find the box on the page
that contains a link, which should look something like `https://github.com/adicu/density.git`.

Copy the link, then open your terminal, navigate to a folder where
you're comfortable keeping coding projects, and run the following
command:

    git clone [link-you-copied]

This will copy the repository and all its contents onto your computer,
and it'll create a new folder inside whatever folder you ran
`git clone` from.

You can do this with any project on GitHub, whether or not it belongs to
you. People who use GitHub to store their projects are participating in
**open source** development, so that everyone can contribute to everyone
else's projects. Now you're entering into that world!

<a id="committing"></a>
### Committing changes to a project

While you should still be saving your work habitually, Git enables you
to create certain checkpoints. Whenever you feel that you've completed a
task, solved a problem, or you just want to save the work that you've
done as a complete unit, you make a Git **commit**.

There are a couple of different steps to doing this. First, let's get
our repository to a state that's ready to be committed. Right now, if
you `ls` or `dir` inside the directory you
just cloned, there should only be one file: README.md. Let's fix that by
adding an `index.html`! You can either reuse your HTML
from our assignments or create something new, but it doesn't matter as
long as you save it in your `username.github.io` folder.

#### `git status`

Now, try running the following command: `git status`. Your
terminal will respond with some information; importantly, it tells us
that we have “untracked files”. Don't worry about the other information
for now.

`git status` is a really important command, because it
shows us what Git thinks the current state of the repository is. It's a
powerful debugging tool, and also helps us understand what other git
commands are actually doing behind the scenes.

#### `git add`

Let's run another command: `git add index.html`. Now, if
we run `git status` again, we'll see that we no longer
have any untracked files; instead, we have a section called “Changes to
be committed”, and it tells us that Git is now aware of a new file
called `index.html`. `index.html` is now
**staged** to be committed.

You can stage all of the files in a directory by running
`git add -A`.

#### `git commit`

So what does it mean for a file to be staged to be committed? It means
that if we run `git commit`, our changes will be included
in that commit, which, like I mentioned before, is essentially a
checkpoint for our repo. Let's do this now by running
`git commit -m "Create index.html"`. Whenever you make a
commit, you include a commit message that explains the changes you've
made, and it goes inside quotes after `-m`.

#### `git log`

If you run `git log`, you'll see the entire history of
your repository. Now that you've committed something, the log will
contain two commits: the initial commit, made on GitHub, and your own
commit, “Create index.html”.

#### `git push`

So far, all of these commands have only been relevant to our local work.
But the magic of Git is that it makes it really easy to share your code
with other people and store it in one centralized location. Run
`git push origin master` and watch the magic unfold! It'll
print some garbage, like
`Delta compression using up to 4 threads`, but what's
important is that it gets your **remote** repository (i.e., GitHub's
version) up to the same point as your local repo. The GitHub page for
your repo will reflect the changes you've made.

<a id="workflow"></a>
### Developing a Git workflow

These commands are all you need to maintain a repo on your own. <span
class="major-key">You should develop a consistent workflow with
Git, and it should look something like this</span>:

1.  Do some good work.
2.  `git add`: Most of the time, you'll use
    `git add -A`, but you can specify individual files if
    need be.
3.  `git commit -m "Extra informative commit message"`
4.  `git push origin master`
5.  Repeat steps 1–4 until code is perfect

#### `git diff`

There's another command that will be helpful to you as you start to work
with bigger and bigger files and projects. Running
`git diff` will show the differences between the lines of
code in your currently saved files and the code from your most recent
commit. If you ever spend more than an hour working on something, you'll
probably find yourself wondering what's actually changed and how it's
changed before you want to `git add` anything. This is a
great way to ensure that you're only committing exactly the code you
want to commit.

--------------

This lesson was a little shorter, but there's still a lot of technical
language to learn!

<a id="terms-git"></a>
### Git terms you should know

Git
:   A version control system developed by Linus Torvalds in 2005.

version control
:   Software that makes it easy to organize and control revisions.

command
:   A program you can run from the command line. You should be familiar
    with `pwd`, `ls` (or
    `dir`), `cd`, and `subl`.

Repository (repo)
:   A folder that contains a project that's tracked by Git.

GitHub
:   A platform that hosts Git projects and facilitates open
    source collaboration.

staged
:   Describes changes that are ready to be committed.
    `git add` stages your changes.

commit
:   A savepoint in Git history.

remote
:   A version of a Git project that is hosted on an outside network.
    GitHub contains the remote version of your username.github.io repo.

Git commands to be familiar with:

:   -   `git status`: current state of the git repo
    -   `git add`: stage files for being committed
    -   `git commit`: save all staged files into a
        definitive savepoint
    -   `git log`: shows commit history
    -   `git push`: pushes local commits to remote
    -   `git diff`: shows difference between repo and most
        recent commit

<a id="project-git"></a>
### Do things with Git

Like I said before, it's really important to develop a consistent workflow with Git. So, now that your `index.html` has been committed, a great way to practice will be to commit the rest of the files you've worked on this week!


#### Committing the rest of your work

You should definitely review the workflow I outlined earlier. You'll need to copy the files and directory structure into your `[username].github.io` folder, then `add`, `commit`, and `push` everything.

Once you've done this, navigate to `[username].github.io` in your browser: surprise!
Now your website is live and viewable to anyone with an Internet connection.
GitHub hosts a free website for all of its users, because they are an
amazing company. If you're interested in customizing your domain name,
we'll talk about it in the next section.

------------------------------
<a href="#top" class="top" id="next-steps">Top</a>
## Level 5: Next Steps

Now that we've learned the basic skills needed to get a website out in
the real world, let's cover some ways to make it better. A lot better.

In no particular order....

<a id="flask"></a>
### Using Flask to build web applications

We've learned a lot of really useful skills over the past few lessons.
However, in order to develop websites that provide services or generate
content dynamically, knowledge of HTML, CSS, and JavaScript isn't quite
enough!

[Flask](http://flask.pocoo.org/) is a Python **framework** that makes it
really easy to take the next step in your illustrious web development
career. For a thorough look at Flask, I can't recommend ADI's own
[guide](http://learn.devfe.st/webdev/) to developing with Flask highly
enough. There's no better way to start making fully-fledged web apps!

<a id="domains"></a>
### Customizing your domain

To customize your website's domain name, it's as easy as 1, 2, 3i, 3ii!

1.  Go to [Namecheap](https://namecheap.com) and buy a domain you like!
    Remember, the [GitHub student developer
    pack](https://education.github.com/pack/) comes with a free
    `.me` domain from Namecheap, in case you don't want to
    spend any money.
2.  In your `username.github.io` repo, at the same level
    as `index.html`create a file called
    `CNAME`. Inside that file, add just one line: your new
    domain name, all lowercase, and nothing else. For example, if you buy `coolperson.me`, your
    site's CNAME is just:

        coolperson.me

3.  In Namecheap, in your dashboard, click “Manage” on the domain name
    you just bought. Then click on Advanced DNS from the tabs in the
    middle of the page. Then, do the following:

    1.  Use the red “Add new record” button to add two A Records, both
        with host `@`, one with the IP address
        `192.30.252.153`, the other with IP address
        `192.30.252.154`.
    2.  Use the red “Add new record” button to add a CNAME Record, with
        host `www` and the value
        `[username].github.io.`.
        Don't
        leave out the dot at the end of it!

You'll need to wait at least half an hour for the changes to finish, but
after that, everything should work like you want it to.

<a id="responsive"></a>
### CSS Media Queries

While you were designing your website, did you ever think about what it
would look like on a phone? More and more people browser the internet
using their phones, and it's our duty as web developers to make sure our
websites' user experience is just as good on a phone or tablet.

The best way to do this is in your CSS, with **media queries**! That's
how this website looks passable on mobile.

-   [Here](http://learnlayout.com/media-queries.html)'s a
    quick introduction.
-   [Here](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)'s
    a great reference guide.
-   [Here](https://css-tricks.com/logic-in-media-queries/) are some
    interesting tricks if you want to get your brain working hard.

<a id="better-js"></a>
### Better JavaScript

Our JavaScript lesson was pretty long, but I still left out a lot of
things that are really crucial for working on anything beyond a personal
site.

1.  I've linked to [Eloquent JavaScript](http://eloquentjavascript.net)
    before, and I'll do it again. It's so important to have good
    JavaScript fundamentals, and this website does by far the best job.
    You should already have read chapters 1 and 2; maybe even more
    important is [Chapter
    3](http://eloquentjavascript.net/03_functions.html), functions.
    Please read that!
2.  MDN also has an excellent [crash
    course](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)
    in all things JavaScript. It's much shorter than EloquentJS, but
    still covers a lot of the important stuff.

<a id="favicons"></a>
### Favicons

Ever wonder how there's a little green J next to the
`title` in your browser's tabs? It's called a **favicon**,
and all the cool kids will have one on their personal sites.

You can make one with [this silly tool](http://www.favicon.cc/), and
store it at the same level as your `index.html` with the
name `favicon.ico`.

To use a `.png`, or to get more information about the
rabbit hole that is the favicon, check out this [incredibly detailed
guide](https://github.com/audreyr/favicon-cheat-sheet). Don't spend too
much time there or your brain will explode.

<a id="ga"></a>
### Google Analytics

Why make a personal site if you can't have incredibly detailed
information about how many people are visiting your website every day,
where they're from, and what browser they're using? [Google
Analytics](https://google.com/analytics) is such a comically useful tool
that every time I use it I'm amazed at how free it is.

The guide on the Google Analytics site should be enough to get you
started;
[here](https://support.google.com/analytics/answer/1008015?hl=en) is an
extra-detailed guide in case you get stuck.

<a id="bootstrap"></a>
### Bootstrap

I love web design, but I recognize that not everyone shares my love for
wrangling with CSS. If that sounds like you, you should check out
[Bootstrap](https://getbootstrap.com): it's a **CSS framework**, which
provides a lot of built-in styling that works well on all devices.

-   [Here](https://www.codecademy.com/courses/web-beginner-en-yjvdd/0/1)
    is a great way to get started with Bootstrap: a lesson from
    Codecademy!
-   [Here](https://getbootstrap.com/getting-started/)'s Bootstrap's own
    “getting started” guide.
-   [Here](https://www.youtube.com/watch?v=YXVoqJEwqoQ)'s a pretty
    reasonable (if slightly out of date) video guide to getting started
    with Bootstrap.

-----------

This concludes the beginner development curriculum! Wow, huh?

Thanks so much for reading all of this stuff. I hope you learned a lot and had fun. If you have any feedback for us, please let us know—we'd love to hear from you!

<script type="text/javascript">console.log("Hi! This is what happens when you console.log from inside a file.");</script>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>

[github]: https://github.com/evantarrh/intro-to-websites.git
[learn]: http://adicu.com/learn
[codecademy]: http://www.codecademy.com
[adi]: http://adicu.com

