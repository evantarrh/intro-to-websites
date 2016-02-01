<style>
.major-key {
  background-color: rgba(255, 215, 48, 0.4);
  padding: 2px 0;
  transition: 0.1s ease background-color;
}

.major-key:hover {
  background-color: rgba(255, 215, 48, 0.7);
}

.image-wrapper {
  text-align: center;
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
    - [1.5 Terms you should know](#terms-html)
    - [1.6 A short project](#project-html)
- [Level 2: CSS](#css)
    - [2.1 What is CSS? What does it look like?](#intro-css)
    - [2.2 Selectors](#selectors)
    - [2.3 How can I customize text with CSS?](#text)
    - [2.4 How do colors work in CSS?](#colors)
    - [2.5 Terms you should know](#terms-css)
    - [2.6 Explore the wonderful world of CSS](#project-css)
- [Additional Resources](#additionalresources)


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
of this page, the text "From Zero To Website" is actually an `h1`, so the code
looks like `<h1>From Zero To Website</h1>`.

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
wanted to link to `evan.land/jade/css.html`, the tag
should look like this: `<a href="/jade/css.html">`. This
means that if you ever just want to link to the homepage (e.g.
`evan.land`), the correct `href` is simply
`href="/"`.

Note that the `href` goes inside the tag itself! This
isn't the only element for which this happens. Another great example is
the `<img>` tag!

<a id="images"></a>
#### The `<img>` tag

It's actually really easy to put pictures on websites—there's a tag for
that!

<div class="image-wrapper">

<img src="http://imgs.xkcd.com/comics/tags.png">

</div>

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

As far as divs go, we'll learn more about them when we move on to styling
our pages with CSS. For now, we can just think of them as organizational tools.

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
`jade/`, and it contains six HTML files. Here are the
files and their respective URLs:

-   `index.html` : `evan.land/jade/`
-   `html.html` : `evan.land/jade/html.html`
-   `css.html` : `evan.land/jade/css.html`
-   `js.html` : `evan.land/jade/js.html`
-   `git.html` : `evan.land/jade/git.html`
-   `nextsteps.html` :
    `evan.land/jade/nextsteps.html`

Note that every page's URL must contain the file name, except for
`index.html`. <span class="major-key">When a folder
contains a file named `index.html`, that is the default
page that will be shown when you don't specify a file name.</span>

Also, this is an interesting case, because the jade folder is really a
folder that lives inside of my personal website. So what the directory
structure really looks like is:

    evan.land/
      - index.html
      - jade/
        - index.html
        - html.html
        - css.html
        - js.html
        - git.html
        - nextsteps.html

There are other files apart from the HTML, so this is a little
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
-   A picture of you. Or of your favorite food. Or your least
    favorite rapper.
-   A paragraph describing yourself. Or your favorite food, or least
    favorite rapper.
-   At least three links to other websites.

___________
<a href="#top" class="top" id="another-section">Top</a>
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
        <p>Fuck Digimon amirite</p>
    </body>

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

font-size: 10px;

font-size: 18px;

font-size: 32px;

Generally, the most readable size for text is around 18 or 20
`px`, but it will depend on the font and the context. Note
that a little change goes a long way when it comes to pixels!

#### line-height

This attribute will control the **line-height** of your text. Again,
we'll use `px` as units. To help show this visually, I've
changed the `background-color` of these next paragraphs,
which we'll talk about soon!

line-height: 15px;\
You don't want your line-height to be less than your font-size.
Readability should always be your priority.

line-height: 20px;\
If your line-height is the same value as your font-size, it still might
look cramped.

line-height: 40px;\
Because double-spacing isn't just for making your essays hit ten pages!
This can look awkward, too, though, so be careful.

Some people believe that the ideal line-height is (font-size × 1.618),
which is the [golden
ratio](https://en.wikipedia.org/wiki/Golden_ratio){.ALMIGHTY-GOLDEN-RATIO}.
It does work remarkarbly well, and it's how the text has been set for
this tutorial all along.

#### font-weight

Font-weight can be a finicky attribute, because it depends on the font
you're using. The two most common values are `400` and
`700` (no units), which translate to "normal" and "bold".
The font I'm using, Lato, also has a 900 weight, which I use for my
`h1`'s.

font-weight: 400;

font-weight: 700;

font-weight: 900;

#### font-style

Font-style should be used as nothing more than an on/off switch for
italics. Relevant values are `italic` and
`normal`.

font-style: italic;

font-style: normal (default value);

#### font-family

Font-family might be the most important attribute, because it lets use
choose our actual font! There are several built-in fonts that will work
in any browser (of which Times New Roman is the most infamous), but we
can do better than that.

font-family: Times New Roman

font-family: Helvetica

font-family: Lato

Lato isn't a built-in font, but I can use it thanks to [Google
Fonts](https://google.com/fonts). Google Fonts gives you free access to
thousands of different fonts, and it's extremely useful. It's easy to
use: once you select a font and some weights, all you have to do is
insert an HTML snippet—which they provide for you—into your website's
`head`! Here's the one I use for this website:

    <link href='https://fonts.googleapis.com/css?family=Lato:400,700,900,400italic' rel='stylesheet' type='text/css'>

That snippet of HTML is all I need to use Lato at different weights.


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

color: rgb(0, 0, 0);

color: rgb(0, 0, 255);

color: rgb(42, 136, 252);

Remember: `rgb(0, 0, 0)` is black and
`rgb(255, 255, 255)` is white.

#### Hex

You should also be familiar with **hexadecimal notation**, or more
simply, **hex values** (or **hex codes**). Here's what it looks like:

color: \#000000;

color: \#0000FF;

color: \#2A88FC;

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

![](https://css-tricks.com/wp-content/csstricks-uploads/firebox.png)

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

<a id="linking"></a>
### How do I put CSS in my HTML file?

Just like HTML, you can write all of your CSS in one file, as long as
you end the filename in `.css`. You can put the file in
the same directory as your HTML files, or create a folder called “css”
and put the file there. Then, in your HTML file, link to the CSS file in
the `head`, using the following syntax:

    <head>
        <title>How Website</title>
        <!-- The href for the CSS will be different depending on
            whether you put the CSS file in a new directory, which is
            what I've done here. -->
        <link rel="stylesheet" type="text/css" href="/css/style.css">
    </head>

A consequence of this is that you can have one CSS file for multiple
HTML files. Once again, that's how this website works! Here's another
look at the directory structure, including the CSS:

    jade/
      - css/
        - style.css
      - index.html
      - html.html
      - css.html
      - js.html
      - git.html
      - nextsteps.html

Each HTML file links to the same CSS file.

An important note is that I also use a font from Google Fonts. <span
class="major-key">To use Google Fonts, you must import the font before
importing the CSS file</span>, like so:

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
using the [snippet from above](#linking). Add a simple rule to your CSS,
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


<a id="another-subsection"></a>
### 2.1 Another Subsection

[github]: https://github.com/evantarrh/intro-to-websites.git
[learn]: http://adicu.com/learn
[codecademy]: http://www.codecademy.com
[adi]: http://adicu.com

