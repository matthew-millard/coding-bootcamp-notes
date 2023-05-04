# Coding Bootcamp Daily Notes

## Table of Contents

- [Day 01](#day-01)
  - [Computational Thinking](#computational-thinking)
  - [Git & Command Line](#git-command-line)
  - [User Story & Acceptance Criteria](#user-story-acceptance-criteria)
- [Day 02](#day-02)
  - [Local Repository](#local-repository)
  - [HTML Attributes](#html-attributes)
- [Day 03](#day-03)
  - [CSS Visibility vs Display Property](#css-properties)
- [Day 04](#day-04)
  -[Media Queries](#media-queries)
  -[Flexbox](#flexbox)
- [Day 05](#day-05)
  -[CSS Reset](#css-resets)
- [Day 06](#day-06)
  -[CSS Grid](#css-grid)
- [Day 07](#day-07)
  -[JavaScritp Basics](#javascript-basics)
- [Day 08](#day-08)
  -[For Loop](#for-loop)
  -[Type Coercion](#type-coercion)
- [Day 09](#day-09)
- [Day 10](#day-10)
- [Day 11](#day-11)
- [Day 12](#day-12)
- [Day 13](#day-13)
- [Day 14](#day-14)
- [Day 15](#day-15)
- [Day 16](#day-16)
- [Day 25](#day-25)
- [Day 29](#day-29)

## Day 01

### Computational Thinking

- Is a way of logically breakdown a problem so that we can develop a step by step solution.

- Break a complex problem into smaller parts, and then developing possible solutions that can be clearly presented in a way that computers and/or humans can understand.

The **Four Cornerstones** of computational thinking are:

- **Decomposition**
      : means breaking down a problem into smaller tasks. Breaking a complex problem into smaller problems or subtasks makes solving the larger problem         more manageable.

- **Pattern Recognition**
      : Thinking about how we've solved these subtasks previously and finding any patterns that might help us to solve this particular problem.

- **Abstraction**
      : Is only focusing on relevant information and that we are disregarding details that won't help us solve this problem.

- **Testing & Debugging Algorithms**
      : An algorithm is essentially a sequence of steps or rules that we can use to solve our problem. Think of it as a set of instructions and a recipe.

### Git Command Line

- `pwd`
  : Print working directory

- `Tab key`
  : Auto complete (case sensitive)

- `mkdir <name of directory>`
  : make new directory

- `rmdir <name of directory>`
  : remove directory

- `rm <file name>`
  : remove file

- `ls`
  : lists all files and directories within the current directory

- `ls -1`
  : same as above, however, lists on individual lines

- `ls -1a`
  : same as above, however, includes any hidden files

- `touch <file name>`
  : add file ls

- `open <file name>`
  : opens file

- `code .`
  : will open directory in Visual Studio Code

- `cd <name of directory>`
  : move into the directory

- `cd` 
  : takes you back to the root directory of the current drive

- `cd ..`
  : takes you back one directory

- `rm -rf .git`
  : removes repository from the directory

- `git init`
  : creates a new repository in the current directory

- `git clone <url>`
  : clones the repository from the remote repository 

- `git branch`
  : let's you know what branch you are working on

- `git add .`
 : will push the current modified or untracked files to the staging area

- `git add -A`
  : will push **all** modified or untracked files to the staging area

- `git remote`
  : tells you if the repository is linked to a remote repository and its name

- `git remote -v`
  : -v stands for verbose. This command will give you the url of the remote repository

- `git remote remove origin`
  : This will remove the link to the remote repository from the local repository

- `git remote add origin <url of remote repository>`
  : This will link the local repository to the remote repository

- `git push -u origin main`
  : This will push the current version of the local repository upstream to the remote repository onto the main branch

- `git checkout <branch name>`
  : to switch to another branch

- `git checkout -b "new branch name"`
  : to switch to a brand new branch

- `git commit -m "commit message"`
  : makes a commit of any files that are in the staging area and adds a commit message

- `git commit` 
  : same as above, except you will be given the option to be able to add a commit message and a description of the commit

- `git cp`
  : copy file(s) and/or directories

- `git pull`
  : downloads latest changes into the local repository, and it also automatically merges change in your working directory. It doesn't give you a chance to review the changes before merging, and as a consequence, 'merge conficts' can and do occur. One **important** thing to keep in mind is that it will merge only into the current working branch. *Other branches will stay unaffected.*

- `git fetch`
  : only downloads latest changes into the local repository. It downloads fresh changes that other developers have pushed to the remote repository since the last fetch and allows you to review and merge manually at a later time using git merge.

- `git merge`
  : the concept of git merging is basically to merge multiple sequences of commits, stored in multiple branches into a single branch. 

### User Story Acceptance Criteria

**User Stories**
When you create websites or web applications, you typically do not work on them in isolation for your own enjoyment. It's more likely that you're creating something that will be used by someone else. The first step then is to identify who that user is. If you start building something without a clear idea of the intended user, you might end up with something functional and pretty that doesn't meet the user's needs. And if it doesn't meet your user's needs, it won't be successful.

That's where user stories come in. A user story is simply a short description of the user you're creating an application for. It ensures that you keep your audience in mind when working on the different parts, or features, of your applications.

A user story consists of the following three sections:

- The type of person using your application
- What the user wants from the application
- Why the user wants what they want (i.e., what problem are they trying to solve?)

Format

- As an ... I want ... so that ...

Ex.

- As a shopper visiting an online store, I want to place items in a shopping cart, so that I can purchase them.

**Acceptance Criteria**
These are the requirements that you must meet to satify the scope of work. They are not exhaustive, but they do entail the minimum aspects of a working solution. Consider this a checklist of baseline requirements.

Acceptance criteria can be presented in various ways. In this case, we'll use a criteria format called scenario-oriented criteria which expresses each requirement in a **When / Then**
format.

---

## Day 02

### Local Repository

There are two ways to setup a local git repository

Clone an existing repository from a remote repository

- To clone an existing repository onto your local machine we have to create a new repository on Github, GitLab or Bitbucket first. Give the repository a name and description. Choose to make it *public or private*. Initialize the repository with a *README file*. Add a .gitignore using a *node* template. Choose a *MIT* license.

- Next we have to establish a link from the remote repository to our local directory where we would like the repository to live. Move into the directory on your local computer where you would like to clone the remote repo to and enter the follow:
`git clone <url>`

- This will do two things. It will make a copy of the remote repo to our local machine and it will also establish a link from our remote repo to our local repo.

Create a local repository on our computer

- Locate the directory that we wish to create the new repository in the terminal.
- Enter the git command `git init`. This will initialize the directory into a repository.
- Hop over to Github and create a new repository. *This time, do not  initialize the repository. Skip this step if you are importing an existing repository.*

- If you would like to create a README.md file in your local repo, use the command line command `touch README.md`.

- If we have any existing files in our local repo, we must stage and then commit these files. To stage the files `git add .` or `git add -A`, this will push all untracked files to the staging area. Next, we have to commit these files `git commit -m "Intial commit"`.

- Next, we have to establish a link from our local repo to our remote repo. In the terminal, type `git remote add origin <url>`. This will create the link to the remote repo that we created earlier.

- Lastly, we need to import our local repo into our remote. Type `git push -u origin main`. This will push the local repo upstream into our remote main branch.

---

### HTML Attributes

>An attribute extends an HTML element, changing its behavior or providing metadata.
>An attribute always has the form `name="value"` (the attribute's identifier followed by its associated value).
>You may see attributes without the equals sign or a value. That is a shorthand for providing the empty string in HTML, or the attributes's name in XML.

ex.

```HTML
<input required />
<!-- is the same as… -->
<input required="" />
<!-- or -->
<input required="required" />
```

---

### CSS Selectors

[Mozilla Attribute Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors)
[Mozilla CSS Selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors)

Basic Selectors

- Universal Selector: `*` will match all the elements of the document.

- Type Selector: selects all elements that have the given node name. `body` `header` `main` `section` `footer` 

- Class Selector: selects all elements that have the given class attribute. `.container` `.card` `.card__content` `card__title` 
The syntax for the class attribute: `class="given-class-name"`

- ID Selector: selects an element based on the value of its `id` attribute. *There should be only one element with a given ID in a document. `#card-1` `#fb-icon` `#linkedin-icon` 
The syntax for the id attribute: `id="given-id-name"`

- Attribute Selectors: select all elements that have the given attribute. `[attr]` `[attr=value]` `[attr~=value]` `[attr|=value]` `[attr^=value]` `[attr$=value]` `[attr*=value]` 

```CSS
/* <a> elements with a title attribute */
a[title] {
  color: purple;
}

/* <a> elements with an href matching "https://example.org" */
a[href="https://example.org"]
{
  color: green;
}

/* <a> elements with an href containing "example" */
a[href*="example"] {
  font-size: 2em;
}

/* <a> elements with an href ending ".org" */
a[href$=".org"] {
  font-style: italic;
}

/* <a> elements whose class attribute contains the word "logo" */
a[class~="logo"] {
  padding: 2px;
}
```

Combinators

- Selector List: a comman-seperated list of selectors. *Both span and div elements will be styled with the border value.*

```CSS
span,
div {
  border: red 2px solid;
}
```

- Single line grouping

``` CSS
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: helvetica;
}
```

- Multi line grouping

``` CSS
#main,
.content,
article,
h1 + p {
  font-size: 1.1em;
}
```

---

## Day 03

### CSS Properties

- The `visibility: hidden;` property is used to specify whether an element is visible or not in a web document, however, it is important to note that the hidden elements take up space in the web document. *The visibility is a property in CSS that specifies the visibility behaviour of an element.*

- The `display: none;`property is used to specify whether an element exists or not on the website. It defines how the components (such as div, hyperlinks, headings, etc) are going to be placed on the web page.

visibility syntax:

```CSS
visibility: visible | hidden | collapse | initial | inherit;
```

Property Values:

- visible: is the default value.
- hidden: the element is not visible, but the layout is still affected. The element may not be seen, but it still keeps the space.
- collapse: hides the element when it is used on a table row or a cell.
- initail: will set the visibility to its default value.
- inherit: it will inherit the property value from its parent element.

display syntax:

```CSS
display: none | inline | block | inline-block;
```

Property Values:

- none: it will not display the element and remove any space it held in the layout.
- inline: is the default value.
- block: it sets the element to block-level.
- inline-block: it sets the element to a block box inside an inline box. This is required often to change an inline element into a inline-block so you can apply top and bottom margins.

Simply put, `display: none;` completely gets rid of the tag, as it had never existed in the HTML page whereas `visibility: hidden;` just makes the tag invisible, it will still sit on the HTML page occupying space, it's just invisible.

---

### Position in CSS

There are 7 values to the **Position** property:

- Static
- Initial
- Inherit
- Relative
- Sticky
- Absolute
- Fixed

---

Static:
Is the default value. The a position property and value is only applied when we want the element to not behave static.
Static basically loads the elements in a top down approach. The elements will be loaded in the sequence they were written.

Relative:
The relative position supports offset properties like (left, right, top, bottom).
So defining the position as relative, then you can offset properties like left, right, top and bottom to move the position of the element which will be relative to its normal position (in the HTML flow) based on those properties.

Absolute:
Absolute positioning allows us to move the element(s) relative to only its parent (non-static position element).
*Note: the parent element does not have to be its direct parent element, it can any ancestor element.*

Lets say we have an image inside a div container. We can move the position of the image using the absolute property with the offset properties relative to the div. Remember the div must not be static position. So we can apply a `position: relative` rule to the div container.

```HTML
<div class="container">
  <img src="./assets/images/random-image.jpg" id="image-1">
</div>
```

```CSS
.container {
  width: 90%;
  max-width: 400px;
  position: relative;
}

#image-1 {
  width: 200px;
  height: 200px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%)
}
```

*The above example would center the image relative to the div container.*

It is important to note that you must be careful while using absolute value, as its hard to maintain an can cause problems with the site's responsiveness.

Fixed:
Fixed behaves similar to absolute but with one clear difference. The position of the element is not relative to the parent element but rather it is relative to the **viewport** (document screen).

- Fixed position is generally used for creating modal popups, sticky navigation bars and footers.

*Note: be careful while using fixed positon as you will be positioning elements directly on the viewport.*

Sticky:
The sticky position is a special position value, as it behaves bot like a *relative* positioned element as well as a *fixed* positioned element.

The element is position relative to the HTML document, but this position changes to fixed, when the element passes a certain scroll point. So the element will stay fixed relative to the viewport. The element will change back to relative, once the element has rollback into the threshold value.
*Note: for fixed to work, an offset value has to be provided like top, bottom, left or right.

Intial:
Is actually a value that overwrites the position value and sets it to the default value static.

Inherit:
The element **inherits** the parent's position value and sets it as its own.

---

Float

- The `float` property specifies whether an element should float to the left, right, or not at all. The default value is none.

*Note: Absolutely positioned elements ignore the `float` property!*
*Note: Elements next to a floating elemetn will flow around it. To avoid this, use the `clear` property of the clearfix hack.*

Syntax:
`float: none | left | right | initial | inherit;`

Clear

- The clear property specifies what should happen with the element that is next to a floating element.

- When we use the float property, and we want the next element below (not on right or left), we will have to use the `clear` property.

The `clear` property can have one of the following values:

- none: This is the default. The element is not pushed below left or right of floated elements.

- left: the element is pushed below left floated element.

- right: The element is pushed below right floated element.

- both: The element is pushed below both left and right floated elements.

- inherit: The element inherits the clear value from its parent.

---

Z Index
`z-index` is a css property that defines the order of overlapping HTML elements. Elements with a higher index will be placed on top of elements with a lower index.

*Note: `z-index` only works on positioned elements (`position: absolute`, `position: relative`, or `position: fixed`).

The default value is auto.
Syntax:
`z-index: 1 | 0 | -5 | 100 | inherit | initial | unset;`

Example:

```HTML
<div class="container">
  <div class="box box--one"></div>
  <div class="box box--two"></div>
  <div class="box box--three"></div>
  <div class="box box--four"></div>
</div>
```

```CSS
.container {
  position: relative;
  width: 600px;
  height: 600px;
  border: 5px solid black;
  background-color: pink;
}

.box {
  position: absolute;
  width: 150px;
  height: 150px;
  border: 3px solid black;
  
}

.box--one {
  background-color: green;
  z-index: 4;
  top: 225px;
  left: 225px;
}

.box--two {
  background-color: red;
  z-index: 3;
  top: 250px;
  left: 250px;
}

.box--three {
  background-color: blue;
  z-index: 2;
  top: 275px;
  left: 275px;
}

.box--four {
  background-color: yellow;
  z-index: 1;
  top: 300px;
  left: 300px;
}
```

![z-index example](./images/z-index-screenshot-example.png)

---

Margin Collapsing

## Day 04

### Media Queries

Media queries ca be used to check many things, such as:

- width and height of the viewport

- width and height of the device

- orientation (landscape or portrait mode)

- resolution

Syntax:
`@media not|only *media type* and (expression) {
  *CSS code*
}`

Example:
```CSS
@media screen and (max-width: 700px) {
  .header {
    flex-direction: column;
  }
}
```

<!-- If the device screen and viewport is 700px or less in width (true) then apply the following css rules within the  -->

Media Types

- all: used for all media type devices

- print: used for printers

- screen: used for all devices with screens

- speech: used for screen-readers


Mobile First Design

Mobile first means designing for mobile before designing for desktop or any other device. 
*Note: This wil make the page display faster on smaller devices.*

Instead of changing styles when the width gets smaller, we should change the design when the width gets larger. This is mobile first design.

The value of the condition at which the media query changes from false to true is known as a breakpoint.

Example:

```CSS
@media screen and (min-width: 400px) and (max-width: 1440px) {
  .main {
    flex-direction: column;
  }
}
```

<!-- The above example has two break points. One at 400px and the other at 1440px. -->

Typical Device Breakpoints
There are tons of screens and devices with different heights and widths, so it is hard to create an exact breakpoint for each device. To keep things simple you could target five groups:

```CSS
/* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px)v {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@meda only screen and (min-width: 600px) {...}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {...}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {...}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {...}
```

### Flexbox

When we apply the CSS property `display: flex;`, there is a whole lot of other properties that will be applied to the child elements. It is as if we wrote these default stylings ourselves:

```CSS
.child {
  flex: 0 1 auto; /* Default flex value */
}
```

The flex property above is a shorthand property. It is the same as:

```CSS
.child {
  flex-grow: 0;
  flex-shrink: 1;
  flex-basis: auto;
}
```

The flex property tells the child elements how to stretch and expand.

Like about it like this:

```CSS
.child {
  flex: [flex-grow] [flex-shrink] [flex-basis];
}

/* or */

.child {
  flex: [max] [min] [ideal size];
}


- `flex-grow: 0;` is the default value. This makes sense as we don't want our elements to expand at all (most of the time).
We normally want the element to grow naturally depending on the content inside it.

If we change the `flex-grow: 1` to all the .child elements, then they will take an equal portion of the .parent element.
*Note: only if the lengths of their contents are the same.*

![Flexbox demo `flex-grow: 1`](./images/Screen%20Shot%202023-03-07%20at%208.17.28%20AM.png)

If you just declare the flex-grow property and not the flex-shrink or flex-basis, not to worry, they will just use their default 
values.

Say we wanted to make one of the .child elements grow more than the others?

```CSS
.child {
  /* flex: 0 1 auto; */
}

.child-1 {
  flex-grow: 3;
}
```

Look at it like this:
`flex: [max] [min] [ideal size];`

Try remember this:

- Use the flex shorthand

- Remember max, min and ideal size when doing so

- Remember that the content of an element can impact how these values work together, too.

## Day 05

### CSS Resets

A CSS reset style sheet is a list of rules that 'reset' all of the default browser styles.

We reset the browser styles for two primary reasons:

- **Not all browsers apply the same default rules.** They may be similar, but not exact.

- Once you start designing and coding all of the fine details of your site, you may discover that a lot of what you are doing is simply **overriding** default browser styles.** The reset does this quickly so that you don't have to.

#### Including the Reset Style sheet using severall different methods.

We can use the reset style sheet as an external style sheet just like we do with our normal styles. 
**Note: It is important that we add it first**, since order matters.

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="style.css">
    <title>Example</title>
</head>
<body>
    
</body>
</html>
```

#### Copy and Paste Into Own Style Sheet

You can also simply copy all of the rules from the reset style sheet and paste them into your own.
**Note: Make sure that you put them at the top so that they don't override any of your rules.**

If you use this method, be sure to clearly mark the reset section of the style sheet and give credit to the author using CSS comments.

#### Normalize Style Sheet

There is a new technique that takes a slightly different approach: normalize.css. Instead of trying to eliminte the default browser styles, the normalize.css instead tries to normalize them to standard values across browsers. This removes some of the downsides of certain copy paste resets such as the **Meyer Reset**. It is also a newer and actively developed stylesheet, so it includes more modern HTML elements.

### Typography

#### Web Fonts

Most people don't ever intentionally install typefaces on their computers. Instead, they simply rely on the typefaces that get installed with the operating system and other software.

Web Safe Fonts

If we ask for a font that the user doesn't have the font will:

- not display.

- A different font is used instead (usually chosen by the browser)

As designers, we **always** want to have control of the font veing rendered.

### Font Stacks

When specifying fonts for web pages, we use a system of 'fallbacks', called a **font stack**

The font stack allows us to:

1. choose the font we want most

2. choose the font we want if the first one isn't available

3. choose any number of other fonts that we might want to fallback on

4. choose a last resort font

This allows us to be sure that we have some control over what font is displayed in our website. Even if the user doesn't have our first choice font, they have some font that **we chose**. 

When selecting your font stacks, you should choose several fonts that are the same type of font (serif, sans serif, slab serif, script, etc.).

You should also consider the spacing and x-height of a typeface. They can look drastically different if not chosen carefully. Additionally, some typefaces will take up much more space than others, causing your layout to differ significantly depending on the typeface rendered.

- Sample comparison of two serif typefaces

- Sample comparison of two sans-serif typefaces

- Real life example with News Gothic

- They should be listed in order of your preference and also by prevalence.

Your second-to-last font choice should be installed on most systems.

The last choice is mostly just there to make sure the right classification of font shows up if all else fails. We hope to never get to this point, but just in case.

### Why should we care about web safe fonts

- Bulletproof fallbacks - we need to specify reasonable alternatives to our custom fonts

- Performance - fonts that are not on a user's computer need to be downloaded and will take longer to load and consume more bandwidth

- Accessibility - web safe fonts have generally been designed for the screen with readability in mind. Other fonts, not necessarily.



## Day 06

### Pseudo Elements

What are pseudo-elements?
A css pseudo element is used to style specified parts of an element.

Common examples:

- Style the first letter, or line, of an element

- Insert content before, or after, the content of an element

Syntax:

```CSS
selector::pseudo-element {
  property: value;
}
```

Ex.

```CSS
h1::first-line {
  font-size: 2em;
  font-family: serif;
}

h2::first-letter { 
  font-size: 2em;
  font-family: serif;
}

.submit-btn::before {
  content: "enter content here";
}

.submit-btn::after {
  content: url(smiley.gif);
}
```

#### Other Pseudo-elements

::marker
The ::marker pseudo-element selects the markers of list items.
So you can style how the list markers look essentially. 

```CSS
::marker {
  color: green;
}
```

::selection
The ::selection pseudo-elemeent allows you to style the look of the selected element, (like if you are to highlight some text
with the cursor) and apply a style to that highlight.

---

### CSS Pseudo Classes

### All CSS Pseudo Classes

- `:active`
  `a:active`
    Selects the active link

- `:checked`
  `input:checked`
    Selects every checked `<input>` element

- `:disabled`
  `input:disabled`
    Selects every disabled `<input>` element

- `:empty`
  `p:empty`
    Selects every `<p>` element that has no children

- `:enabled`
  `input:enabled`
    Selects every enabled `<input>` element

- `:first-child`
  `p:first-child`
    Selects every `<p>` elements that is the first child of its parent

- `:first-of-type`
  `p:first-of-type`
    Selects every `<p>` element that is the first `<p>` element of its parent

- `:focus`
  `input:focus`
    Selects the `<input>` element that has focus

- `:hover`
  `a:hover`
    Selects links on mouse over

- `:in-range` `input:in-range`
    Selects `<input>` elements with a value within a specified range

- `:invalid`
  `input:invalid`
    Selects all `<input>` elements with an invalid value

- `:lang`(language)
  `p:lang(it)`
    Selects every `<p>` element with a lang attribute value starting with "it"

- `:last-child`
  `p:last-child`
    Selects every `<p>` elements that is the last child of its parent

- `:last-of-type`
  `p:last-of-type`
    Selects every `<p>` element that is the last `<p>` element of its parent

- `:link`
  `a:link`
    Selects all unvisited links

- `:not(selector)`
  `:not(p)`
    Selects every element that is not a `<p>` element

- `:nth-child(n)`
  `p:nth-child(2)`
    Selects every `<p>`element that is the second child of its parent

- `:nth-last-child(n)`
  `p:nth-last-child(2)`
    Selects every `<p>` element that is the second child of its parent, counting from the last child

- `:nth-last-of-type(n)`
  `p:nth-last-of-type(2)`
    Selects every `<p>` element that is the second `<p>` element of its parent, counting from the last child

- `:nth-of-type(n)`
  `p:nth-of-type(2)`
    Selects every `<p>` element that is the second `<p>`element of its parent

- `:only-of-type`
  `p:only-of-type`
    Selects every `<p>` element that is the only `<p>` element of its parent

- `:only-child`
  `p:only-child`
    Selects every `<p>` element that is the only child of its parent

- `:optional`
  `input:optional`
    Selects `<input>` elements with no "required" attribute

- `:out-of-range`
  `input:out-of-range`
    Selects `<input>` elements with a value outside a specified range

- `:read-only`
  `input:read-only`
    Selects `<input>` elements with a "readonly" attribute specified

- `:read-write`
    `input:read-write`
    Selects `<input>` elements with no "readonly" attribute

- `:required`
  `input:required`
    Selects `<input>` elements with a "required" attribute specified

- `:root`
    Selects the document's root element

- `:target`
    `#news:target`
    Selects the current active #news element (clicked on a URL containing that anchor name)

- `:valid`
  `input:valid`
    Selects all `<input>` elements with a valid value

- `:visited`
    `a:visited`
    Selects all visited links

---

### CSS Combinators

A combinator is something that explains the relationship between the selectors.

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

- descendant selector (space)

- child selector (>)

- adjacent sibling selector (+)

- general sibling selector (~)

#### Descendent Selector

The descendant selector matches all elements that are descendants of a specified element.

*Note: VS Code has a awesome tooltip when you hover over the selector in the editor. It will inform you the parent element and then which child(s) are getting selected.*

```CSS
div p {
  color: red;
}
```

#### Child Selector

The child selector selects all elements that are the children of a specified element.

This is best shown with an example:

```CSS
div > img {
  width: 50%;
}
```

The above example will apply a width of 50% to all images that are child element of a div element.

#### Adjacent Sibling Selector (+)

The adjacent sibling selector is used to select an element that is directly after another specific element.
Sibling elements must have the same parent element, and "adjacent" means "immediately following".

The following example selects the first `<p>` element that are placed immediately after `<div>` elements:

```CSS
div + p {
  background: green;
}
```

The above code would select the very next `<p>` element that is a sibling of a `<div>`.
*Note: Important, it will select the **SIBLING** element, not a **CHILD**.*

#### Genral Sibling Selector (~)

The general sibling selector selects all elements that are next siblings of a specified element.

The following example selects all `<p>` elements that are next siblings of `<div>` elements:

```CSS
div ~ p {
  color: red;
}
```

---

### CSS Grid

---

## Day 07

### JavaScript Basics

Data types:

1. String: String represets text data in js. You can use singular quote marks ('') or double quote marks ("") to create a string.

2. Number: 44 - A number represents numeric data. You can add `+`, subtract `-`, multiply `*`, divide `/` and find the remainder with modulus `%` operator.

3. Boolean: true | false - Booleans can only either be `true` or `false`.

4. Null: null is a value that is used to indicate “nothingness”. Developers need to explicitly set a value to be null.

5. Undefined: undefined is a value that indicates an absence of a value. We say that something is undefined when it is not explicitly defined.

7. Symbol: a symbol is a new primitive that comes with ES6. You don't need symbols 99% of the time. They are meant for a very unique use case.

8. BigInt: stands for Big Integer. It lets you create extremely large numbers (that cannot be supported by `Number`)

***Note: Null is different from undefined. If you compare null and undefined with the strictly equal operator, you’ll get false.***

#### String Concatenation

Strings can be added together with the + operator. 
`console.log('Matthew ' + 'Millard')`
// Matthew Millard

#### Declaring Variables

The variableName
variableName is the name of the variable you’re declaring. You can name it anything, as long as it follows these rules:

- It must be one word
- It must consist only of letters, numbers or underscores (0-9, a-z, A-Z, _).
- It cannot begin with a number.
- It cannot be any of these reserved keywords
- If you need to use two or more words to name your variable, you should join the words together, but capitalize the first letter of each subsequent word. This weird capitalization is called camel case.

- The value
The value is what you want the variable to be. It can be a primitive (like a string and a number etc) or an object (like an array or function).

- `=` in JavaScript
= in JavaScript doesn’t work like = in Math. Don’t get confused.

In JavaScript, = means assignment. When you use =, you set (or assign) the value on the right hand side (RHS) of the = sign to the left hand side (LHS) of the = sign.

- Evaluation before assignment
Variables can only take up one value each. If you have an equation that needs to be evaluated on the RHS, it must be evaluated before it can be assigned to a variable.

#### const vs let vs var

- `const` and `let` are keywords made available to us in ES6. They are better keywords to create variables than `var`.

- const: If you declare a variable with const, you cannot assign it with a new value.

- let: If you declare a variable with let, you can assign it with a new value.

### If/else Statements

``` javascript
if (condition === true) {
  // Then run this code block and exit.
} else if (condition === true) {
  // Then run this code block and exit.
} else {
  // If they both do not evalute to true, then run this code block.
}
```

If the first condition evaluates to true, JavaScript executes the code in the if block.

If the first condition evaluates to false, JavaScript checks the condition in the next else if block and see whether it evaluates to true. It goes on and on until all else if blocks are exhausted.

To check whether a condition evaluates to true or false, JavaScript relies on two things:

Comparison operators
Truthy and falsey values.

#### Comparison Operators

There are four main types of comparison operators:

Greater than (>) or greater or equals to (>=)
Smaller than (<) or smaller or equals to (<=)
Strictly equal (===) or equal (==)
Strictly unequal (!==) or unequal (!=)

=== vs == (or !== vs !=)
JavaScript is a loosely-typed language. What this means is that, when we declare variables, we don’t care what type of value goes into the variable.
You can declare any primitive or object, and JavaScript does the rest for you automatically.

When comparing things with strictly equal (===) or strictly unequal (!==), JavaScript checks two things:

- The type of the variable

- The value of the variable

When comparing things with equal (==) or unequal (!=), JavaScript converts (or casts) the types so they match each other.

- ***Generally, JavaScript tries to convert all types to numbers when you use a comparison operator. The string 24 is converted into the number 24 before the comparison. That’s why a string of 24 equates to a number of 24 when you use ==.***

- Booleans can also be converted into numbers. When JavaScript converts Booleans into numbers, true becomes 1 and false becomes 0.

***Important: Automatic type conversion (when using comparison operators) is one of the common causes of hard-to-find bugs. Whenever you compare for equality, always use the strict versions (=== or !==).***

- In JavaScript, each object has a “identity card”. This identity card is called the ***reference*** to the object. When you compare objects with equality operators, you’re asking JavaScript to check if the two objects have the same reference (same identity card).

#### Truthy and Falsey

Truthy and Falsey
If you write a single variable as the condition of an if/else statement, JavaScript checks for a truthy or a falsey value.

``` javascript
const numApples = 135

if (numApples) {
  // Eat an apple
} else {
  // Buy an apples
}
```

- A falsey value is a value that evaluates to false when converted into a boolean. There are six possible falsey values in JavaScript:

1.false
2.undefined
3. null
4. 0 (numeric zero)
5. "" (empty string)
6. NaN (Not A Number)

A truthy value, on the other hand, is a value that evaluates to true when converted into a Boolean. In the case of numbers, anything that’s not 0 converts to true.

Automatic type conversion to truthy and falsey values are highly encouraged in JavaScript, because they make code shorter and easier to comprehend.
For example, if you want to check if a string is empty, you can use the string in the condition straightaway.

#### The NOT Operator

- The NOT operator (!) flips truthy and falsey values around. Truthy values becomes false while falsey values become true.

The NOT operator can be used to eliminate else statements, like this:

``` javascript
const str = ''

if (!str) {
  // Only do something if string is empty (NOT truthy)
}
```

## Day 08

### Loops

#### For Loop

A for loop runs a block of code as many times as you want to.
Here's a for loop that logs each value in the array:

``` javascript
const myArray = ['Matthew', 'Millard', 34, 'Scotland', true]
for (let i = 0; i < myArray.length; i++) {
    console.log(myArray[i])
}
```

``` javascript
const numbers = [25, 22, 12, 56, 8, 18, 34]
for (let i = 0; i < numbers.length; i++) {
  const num = numbers[i]
  if (num < 20) {
    console.log(num + ' is less than 20!')
  }
}
```

***Infinite loops: Infinite loops occur when the condition for a loop always return true. Your browser will hang if you run an infinite loop.***

Looping through Arrays

In practise, you always loop through an array or object. When you loop (or iterate) through an array, you go through each item in the array once.
To do so, you can use the length of the array as a condition like both the examples above.

You can also write a for loop with a negative incrementExpression. It runs faster than the positive incrementExpression version, but loops from the last item. Use this if you need to run a super performant app.

``` javascript
for (let i = myArray.length -1; i >=0; i-- ) {
  // run code here.
}
```

#### The 'for of' loop

A (much better) way to loop through an array to use a for...of loop. This is a new loop syntax that comes with ES6. It looks like this:

``` javascript
const myFamily = ['Hamish', 'Finn', 'Islay', 'Amy', 'Matthew']
for (let person of myFamily) {
  console.log(person)
}
```

#### The forEach loop

All arrays contain a forEach method. It helps you loop through every item in an array in a simple-to-read manner.

Syntax:

``` javascript
array.forEach((currentValue, index, array) => {
  // Your loop here
})
```

- currentValue: refers to the current item in the array.

- index: is the position of the item within the array. The first item has an index of 0; the second, an index of 1; and so on.

- array: refers to the array that you're looping over. Your don't need this argument most of the time.

``` javascript
const myFamily = ['Hamish', 'Finn', 'Islay', 'Amy', 'Matthew']

myFamily.forEach(person => {
  console.log(person)
})
```

``` javascript
myFamily.forEach((familyMember, index) => {
    console.log(`${familyMember} has an index of ${index} in the array.`)
})
```

#### For...of vs forEach

You can use either for...of or forEach to loop through all arrays. They do the same thing. I highly suggest you learn forEach properly.

I prefer forEach because it’s easier to read, shorter to write, which means it’s more maintainable and has less room for bugs to hide.

Furthermore, forEach is a good base to help you learn more advanced array methods like map, filter, reduce, find, some and every. Each method mentioned does a specific thing that’s way more useful than forEach or even for...of.

#### While Loop

A while statement will create a loop around a code block that will continue to iterate and execute that code block as long as the condition remains true.
As soon as the condition evalutes to false, the loop cycle breaks and exits the loop.

Syntax:

``` JavaScript
while (condition) {
  //code block to be executed
}
```

Example:

``` JavaScript
cars = ['bmw', 'ferrari', 'aston martin', 'mercedes benz', 'renault', 'fiat',]
let i = cars.length -1
while (i >= 0) {
  console.log(cars[i])
  i--
}
```

---

### Logical Operators

#### AND && operator

The logical AND (&&) operator will evalute and pass as true if **ALL** operands are true. Otherwise it will be false.

``` JavaScript
const name = 'Matthew'
const lastName = 'Millard'

if ( name === 'Matthew' && lastName === 'Millard' {
  // code block will run, as both operands evalute to true.
})
```

#### Logical NOT (!)

The logical NOT ( ! ) operator takes truth to falsity and vice versa. It will invert a truthy value to a falsey value for example or vice versa.

``` javascript
if (!false) {
  // code block will run.
}
```

False becomes true, so the code block will run.

#### Logical OR ( || )

The logical OR operator for a set of operands is true if and only if one or more of its operands is true.

``` javascript
const a = 5
const b = -5

if ( a > 0 || b > 0 ) {
  // if one of the operands evalute to true, this code block will run. 
}
```

---

### Type Coercion

Type coercion is converting from one data type to another.

#### Explicit Type Coercion

Example:

``` JavaScript
let a = '1' // String data type
a = parseInt(a) // parseInt will convert the string value of '1' to the number data type with the value of 1.
```

***This is called explicit type coercion, as we are explicitly saying we wish to convert this string into a number.***

Use the function parseFloat() if you wish to have a decimal number. If not, parseInt will convert to a whole number.

To convert a number into a string, we would use the `toString()` function. 
Ex.

``` JavaScript
let a = 1.34
a = a.toString()
console.log(typeof a) // String will be logged in the console.
```

Implicit Type Coercion
This means the computer is taking the type coercion for you automatically. You are not telling the computer to do the type coercion, it is doing it
on its own.

Generally, when you are dealing with javascript, the best rule of thumb is to always explicitly convert your data types so they are exactly the same, so you don't run into weird bugs related to type coercion.

## Day 09

### Function Declaration vs Function Expression

Function Declaration:

``` JavaScript
function getUser(name, age, sex) {
  // run code.
}
```

Function Expression:

``` JavaScript
const user = function getUser(name, age, sex)
```

Arguments Vs Parameters
Quite often these are used interchangeably, however, technically **parameters give a name to the data** and **arguments give a value to the data**.

### Hoisting

### Scope

When you have a set of curly braces {}, this is defining a new local scope. You have global scope, and within that, you have local scopes.
A local scope, like within a function can access values in the global scope. However, it works like a one way door, as the outer global scope cannot access values within a local scope.

Lets say you have a variable with the name user. `const user = 'Matthew'` defined within a function, and you also had a variable defined as user in the global scope. This won't cause any conflicts as the outer scope cannot see within the local scope and the local scope will always look for the user value within before looking into the outer scope.

### Closures

Simply put, normally referred to as functions within functions.
ex.

``` JavaScript
function func(variable) {
  const variable3 = 3
  return function func2(variable2) {
    console.log(variable)
    console.log(variable2)
    console.log(variable3)
  }
}


cont a = func(1)
a(2)
```

### New And This

## Day 10

### Selecting An Element

`querySelector` method:
The document object contains a method called `querySelector`. It can look like this:

``` JavaScript
const element = document.querySelector(selector)
```
The selector refers to the id, class, tag, or attribute of the element you want to select. These selectors are written the same way as you would write selectors in CSS:

- To select an element with an id, you prepend it with `#`

- To select an element with a class, you prepend it with `.`

- To select an element with an attribute, you would write the attribute in square `[]` brackets

Example:

``` JavaScript
document.querySelector('#password')
```

*querySelector returns only one element and that the element will be the first element it finds - it doesn't matter how many elements you selector matches.*

If you want to select multiple elements, you'll need to use another method called `querySelectorAll`.

You can write complex selectors that combine id, classes, tags and even attributes, but don't do it - one selector is usually good enough to handle your selection needs.

``` javascript
// Dont't do this
document.querySelector('header#logo')
```

All elements have the `querySelector` method too.
This lets you search for an element within another element - so JavaScript doesn't have to comb through the entire DOM.

When you use `element.querySelector`, you'll write that much easier to read and understand, less prone to bugs, and faster compared to using `document.querySelector` all the time.

### Changing Classes

Yes, you can change CSS with JavaScript, but you don't want to do it often.
For now, you'll want to change CSS with classes because that's the best way to do it - let CSS handle CSS stuff.

#### Adding a class

To add a class, you use the `add` method. This method can be found within the classList property that exists for all elements.

``` JavaScript
element.classList.add('className')
```

#### Adding multiple classes at once

You can add multiple classes to the same element if you pass in extrea arguments, like this:

``` JavaScript
element.classList.add('firstClass,' 'secondClass', 'thirdClass')
```

*Note: There's no need to add multiple classes in practise. One class is good enough, provided you're smart with your classes.*

#### Removing a class

To remove a class, you use the `remove` method, which is present in `classList`.

``` JavaScript
element.classList.remove('className')
```

Note: You don't need to add `.` before your classes when you use `element.classList`. This is a common mistake if you mix up the syntax for `querySelector` and `element.classList`.

#### Checking if a class exists

If you want to check if a class exists, you can use the `contains` method:

``` JavaScript
element.classList.contains('className')
```

NOTE: This method is often used together with the `if` statement to check whether the class exists:

``` JavaScript
if (div.classList.contains('header')) {
  // code block
}
```

#### Toggling a class

Toggling classes means this:

- Remove `className` if `className` exists

- Add `className` if `className` doesn't exist

Note: You'll toggle class on/off frequently when you build components - so much that javascript provides you with a `toggle` method.

``` JavaScript
element.classList.toggle('className')
```

---

### The BOM and the DOM

BOM stands for Browser Object Model while DOM stands for Document Object Model.

#### BOM

The BOM refers to the set of JavaScript objects browsers provide you with. It gives you the `window` object in JavaScript. If you open up your inspector and write `console.log(window)`, you'll see the list of every JavaScript method you can use.


## Day 11

### The Date Object

```JavaScript
const date = new Date()
```

In JavaScript, we can tell the date and time with the `Date` object.

If you console.log date, you'll get a log that tells your four things:

- The day of the week

- The date today

- The time now

- The timezone

#### Built-in Formats

Date comes with seven methods that lets you convert a `Date` object into a string. Here's what each of them do:

1. `toString` returns: Wed Jan 23 2019 17:23:42 GMT+0800 (Singapore Standard Time)

2. `toDateString` returns: Wed Jan 23 2019

3. `toLocaleString` returns: 23/01/2019, 17:23:42

4. `toLocaleDateString` returns: 23/01/2019

5. `toGMTString` returns: Wed, 23 Jan 2019 09:23:42 GMT

6. `toUTCString` returns: Wed, 23 Jan 2019 09:23:42 GMT

7. `toISOString` returns: 2019-01-23T09:23:42.079Z

*Note: Each method gives a specific date/time string. Unfortunately, none of them gives us the format (23 Jan, 2019) we wanted. We need tot create the format ourselves with some Date methods.*

#### Date Methods

Here's a list of methods that helps you format a date.

1. `getFullYear`: Gets 4-digit year according to local time.

2. `getMonth`: Gets month of the year (0-11) according to local time.

3. `getDate`: Gets day of the month (1-31) according to local time.

4. `getDay`: Gets day of the week (0-6) according to local time. Day of the week begins with Sunday (0) and ends with Saturday (6).

#### Creating a custom format

First, we need to create a date object.

`const today = new Date()`
// Tue Mar 28 2023 09:56:16 GMT-0400 (Eastern Daylight Saving Time)

Then, to get the day of the month we can do the following:

`const day = today.getDate()`
// 28

`const year = today.getFullYear()` // 2023

*Note: Getting the likes of the name of the month is harder and requires more code.*

We only have access to `getMonth`, and `getMonth` returns a number from 0 to 11. This means we must convert the month number (0-11) into a month string (January-December) ourselves.

First, we need to create an object that tells us 0 is January, 1 is February etc..

``` JavaScript
const monthsInAYear = [
  'January',
  'February',
  'March',
  'April',
  'May',
  'June',
  'July',
  'August',
  'September',
  'October',
  'November',
  'December',
]
```

Let's get the name of the current month:

``` JavaScript
const monthIndex = today.getMonth()
const monthName = monthsInAYear[monthIndex]
console.log(monthName) // January
```

#### Getting day of the week

What if we wanted to get `Tuesaday, 28 March` instead?

The `Date` object has a `getDay` method that tells us the day of the week. It returns a number from 0 to 6. The values goes like this:

- 0: Sunday

- 1: Monday

- 2: Tuesday

- 3: Wednesday

- 4: Thursday

- 5: Friday

- 6: Saturday

If we want to get `Tuesday` from `Date` we need to create a `daysInAWeek` array that converts number into strings.

``` JavaScript
const dayString = daysInAWeek[today.getDay()]
console.log(dayString) // Tuesday
```


### For in... loop

The JavaScript `for in` statement loops through the properties of an Object:

Syntax:

``` JavaScript
for (key in object) {
  // code block to be executed
}
```

For In Over Arrays
The JavaScript `for in` statement can also loop over the properties of an Array:

Syntax:

``` JavaScript
for (variable in array) {
  // code
}
```

Example

``` JavaScript
const person = {
  Name: 'Matthew',
  Age: 34,
  Gender: 'Male'
}

for (let x in person) {
  console.log(person[x])
}
// Matthew
// 34
// Male
```

Example Explained

- The for in loop iterates over a **person** object

- Each iteration returns a **key** (x)
- The key is used to access the **value** of the key
- The value of the key is **person[x]**

*Note: The `for in` statement can also loop over the properties of and array.*

*Important! Do not use `for in`  over an array if the index order is important. It is better to use a `for of`, `.forEach()` or `for` loop when the order is important.*

#### Map() Array methods

The difference between .forEach() vs. map()

Example
If we use a .forEach() method to iterate through an array and log each value to the console:

``` JavaScript
const studentName = ['Matthew', 'Oliver', 'Benny', 'Ginette', 'Amy', 'Donald']

studentName.forEach(student => console.log(student.toUpperCase()))

// MATTHEW
// OLIVER
// BENNY
// GINETTE
// AMY
// DONALD
```

We could do the exact same thing with a map() method.

``` JavaScript
const studentName = ['Matthew', 'Oliver', 'Benny', 'Ginette', 'Amy', 'Donald']

studentName.map(student => console.log(student.toUpperCase()))

// MATTHEW
// OLIVER
// BENNY
// GINETTE
// AMY
// DONALD
```

As you can see there is no difference. However, say we want to assign the values to an new array.

``` JavaScript
const newArray = studentName.forEach(student => student)
console.log(newArray)

// undefined
```

As you can see the .forEach method returns `undefined`.

``` JavaScript
const newArray = studentName.map(student => student)
console.log(newArray)

// [ 'Matthew', 'Oliver', 'Benny', 'Ginette', 'Amy', 'Donald' ]
```

With the `map()` method we are returned an array with the student names.
This is because map() returns a new array without altering our intial array. While `.forEach()` does not return a new array.

*This is the key difference between the two methods.*

It is important to note, that map() will return a new array and will not the original array. We can check this if we `console.log(studentNames)`

## Day 12

### Sort() Method

The `.sort()` method returns an aray with its items sorted in place.

``` JavaScript
// No parameters
array.sort()

// With optional function
array.sort((firstElement, secondElement) => {
  // function  body
})
```

If the `.sort()` method is used  with no arguments, all items with undefined values are shifted to the end of the array while the remaining items are converted to strings and sorted by **Unicode code point value**.

An optional function is used to define how items are sorted. **This is done by iterating over the array and comparing every `firstElement` and `secondElement` in the function body.**

Example
In the following example, the `.sort()` method is applied to two arrays, `letters` and `numbers`.

``` JavaScript
const letters = ['d', 'b', 'e', 'a', 'c']
const numbers = [5 , 2, 123, 5.01, 43.5]
```

This results in the following output:

``` JavaScript
letters: ['a', 'b', 'c', 'd', 'e']
numbers: [123, 2, 43.5, 5, 5.01]
```

The letters were sorted in alphabetical order. The items in numbers were sorted based on the leading number in the item's value (e.g Unicode value). Sorting numerical values more strictly requires a custom comparison function.

Example using the optional function:
The  following example showcases how the optional `callback` argument can be used to sort a `numbers` numbers array in ascending and descending order:

``` JavaScript
const ascending = numbers.sort((a,b) => a - b)

console.log(ascending) // [2, 5, 5.01, 43.5, 123]
```

``` JavaScript
const descending = numbers.sort((a,b) => b - a)

console.log(descending) // [123, 43.5, 5.01, 5, 2]
```

### findIndex() Method

`findIndex()` lets you *find the index of an item in an array*. It **loops through every item in the array and returns the first truthy expression**.

The syntax looks like this:

``` javascript
const index = array.findIndex((currentItem, index) => {
  // return a truthy expression here...
})
```

Its much easier to explain Array.findIndex with an example, so let's do that. Let's say you have an array of objects. Each object is a person, and each person has a name.

``` javascript
const people = [
	{
		name: 'Matthew',
	},
	{
		name: 'Amy',
	},
	{
		name: 'Donald',
	},
	{
		name: 'Ginette',
	},
]
  ```

You want to know the position of the person named `Donald` in the `people` array. To do so, you can use `person.findIndex()` and check if the `name` property in each object matches `Donald`.

const indexOfDonald = people.findIndex(person => person.name === 'Donald')

console.log(indexOfDonald) // 2

### find() Method

`find` works the same way as `findIndex`, but `find` returns the item instead of the index.

```javascript
const donald = people.find(person => person.name === 'Donald')
console.log(donald)
// {name: 'Donald'}
```

### filter() Method

`array.filter` **returns a new array** that contains a subset of the original array. **Items will be added to the new array if you return a truthy expression**.

``` javascript
const filteredItems = array.filter((currentItem, index) => {
  // return a truthy expression to include in filteredItems
})
```

Once again, its easier to explain `filter` with an example, so let's do that.

Let's say you have a list of numbers. You want to make another list of numbers that are bigger than ten. You can do this easily with `filter`.

``` Javascript
const numbers = [1, 12, 4, 18, 9 , 7, 11, 3 , 50, 5, 6]
const numsGreaterThanTen = numbers.filter(num => num > 10)
console.log(numGreaterThanTen) // [ 12, 18, 11, 50 ]
```

### reduce() method

The `.reduce()` method combines each element of an array, using a specified reducer function, and returns a single value.

Another definition: `reduce` is an array method that helps you convert an array into a single value. It looks like this: 

``` javascript
const callback = (accumulator, currentValue, index) => {
  // return something here
}

const result = array.reduce(callback, initialValue)
```

**initialValue** is the value you want to start with.

**accumulator** is the value returned from the previous iteration. It will be `initialValue` for the first iteration.

**currentValue** is array item in the current iteration.

Let's go through some examples.

#### Summing Numbers Example

Let's say you have a list of numbers. You want to find the total sum of these numbers.

`const numbers = [1, 2, 3, 4, 5, 6, 7,]`

Here's the code to sum the numbers.

``` JavaScript
const total = numbers.reduce((acc, num) => {return acc + num}, 0)
```

Let's go through what happens, step by step.

First, you pass an `initialValue` to `reduce`. This initialValue should be 0 because:

1. We want `accumulator` to be a number.

2. We don't want the `initialValue` to affect the sum.

**NOTE: `accumulator` will be `initialValue` in the first iteration. `currentValue` will be the first array item.**

You need to return a value in the callback. This value will be used as the next `accumulator`. Since we want to sum numbers, we return the sum of `accumulator` and `currentValue`.

`accumulator` takes on the returned value in the second iteration.
`currentValue` will be the second array item.

We return the sum of the two values we have, `accumulator` and `currentValue`. This process goes on until reduce loops through the entire array. **The final value will be returned to the function call.**

Below is an example using the reduce method to help get the average age.

``` JavaScript
const ages = [1, 12, 4, 18, 9, 7, 11, 3, 50, 5, 6]

// I want to find the average age
const averageAge = getAverageAge(ages)

function getAverageAge(arr) {
	const sumOfAges = arr.reduce((acc, age) => {
		return acc + age
	}, 0)
	const averageAge = sumOfAges / arr.length
	return Math.round(averageAge)
}
console.log(averageAge) // 11
```

#### Reducing an array into an object

We'll create the `reduce` method together for this example.
Let's say we have an array of fruits. We want to know the number of each type of fruit.

``` JavaScript
const fruits = ['apple', 'apple', 'banana', 'banana', 'orange', 'pear', 'apple']

const tally = fruits.reduce((acc, fruit) => {
	if (acc[fruit]) {
		acc[fruit] = acc[fruit] + 1
	} else {
		acc[fruit] = 1
	}
	return acc
}, {})

console.log(tally)
// { apple: 3, banana: 2, orange: 1, pear: 1 }
```

Let's clean up the reduce function next. We can do so with ternary operators.

``` JavaScript
const tally = fruits.reduce((acc, fruit) => {
	const fruits = acc[fruit]
	fruits ? (acc[fruit] = fruits + 1) : (acc[fruit] = 1)
	return acc
}, {})
// { apple: 3, banana: 2, orange: 1, pear: 1 }
```

#### Flattening an array









## Day 13

### Third Party API

jQuery API

jQuery is a fast, small, and feature-rich JavaScript libaray. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers.

To add jQuery API, we have to include the CDN in our HTML document.

``` HTML
 <head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
</head>
```

How to create an element:
`$('<h1>')`

How to add text content:
`element.text('Hi there')`

How to add a attribute to an element:
`element.attr('class', 'header')`

How to add a class to an element:
`element.addClass('container')`

How to add css styling to an element:
`element.css('background-color', 'red')`

How to append a child element onto an element:
`element.append('<h2>')`

How to add an event listener to an element:
`element.click(function () {
  // do stuff...
})`

How to select an HTML element:
`var button = $('.button')`

How to get the value of an input:
`const input = $('#usernameInput')
const userName = input.val()`

*Note: You can log to the console `console.log($())` to see a list of all the methods available to use.*

All the methods available in jQuery are listed in the documention on the website.
[jQuery Documention](https://api.jquery.com/)

#### Event Delegation

Let's say you have a list of items. You want to listen to a `click` event on each item. One way is to attach an event listener to every item.

Example

``` JavaScript
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
  <li>Item 5</li>
</ul>
```

Most likely you would think to use a forEach() method as below:

``` JavaScript
const items = Array.from(document.querySelector('li'))

items.forEach(item => {
  item.addEventListener('click', () {
    // do stuff here...
  })
})
```

But what if you had one thousand items? If you do the above, you'll create one thousand event listeners. That's not the best way.

A better way is to use the event delegation pattern.

#### Event Delegation Pattern

The event delegation pattern makes use of event propagation. It works like this:

1. You attach one event listener to an ancestor element

2. Ancestor element listens toa all events in descendant elements

*Note: the event delegation pattern only works for events that bubble.*

``` HTML
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
  <li>Item 4</li>
  <li>Item 5</li>
</ul>
```

``` JavaScript
const list = querySelector('ul')

list.addEventListener('click', e => {
  // do stuff here...
})
```

Determining the event target

The element that fires the event is called the *event target*. It can be found with the `target` property.

``` JavaScript
list.addEventListener('click', e => console.log(e.target))
```

Avoid misfires
The event delegation pattern is sensitive to all events fired from the listening element onwards. In this case, you can also fire the callback when you click on the list itself.

To prevent such misfires from happening, we need to check if the target element matches the element we're looking for. We can do so with the `matches` method.

`matches` checks if the element matches the selector we provided. You should be familiar with it's syntax.

``` JavaScript
element.matches(selector)
```

`matches` will either return `true` or `false`. It will be true if the element matches the `selector`.

In this case, we only want to do something if a user clicks on a list item. We can check whether the event target is a list item with `matches`.

``` JavaScript
list.addEventListener('click', e => {
  if (e.target.matches('li')) {
    // do stuff here...
  }
})
```

## Day 16

### Fetch API

The fetch API can even request data from third-party API's, like the OpenWeather API.

`fetch()` A modern way for the client (browser) side to exchange data with a server.

When the client makes a request to the API server, the request enters a pending state. Then when the server sends back a response, and everything has worked as expected, the response is going to be resolved and the data the client gets is then usable.

Sometimes a response comes back with errors. In this case, the fetch request is then rejected.

``` JavaScript
fetch(requestUrl)
.then(function (response) {
  return response.json()
})
```

Now, when this URL gets sent through, the fetch requests this is where the pending state happens and it is either going to be resovled or rejected.

If it is resolved, then I am going to do something with that response.

The response is just an HTTP response. It is not JSON. You need to extract the JSON body from this response.

So by using this method, I'm able to extract the JSON from this response.
`return response.json()`

Now that you hvae converted the HTTP response to JSON, we ***then*** need to do something with this ***data***.

``` JavaScript
const requestUrl = 'http://ergast.com/api/f1/2008/5/results'
// make sure to wrap the url in quotes.

fetch(requestUrl)
.then(function (response) {
  return response.json()
})
.then(funtion (data) {
  console.log(data)
  // do something now with the data.
})
```

Before we move on, lets look at a few way this fetch() function may be written. The below example uses arrow functions to reduce the amount of code.

``` JavaScript
const requestUrl = 'http://ergast.com/api/f1/2008/5/results'

fetch(requestUrl)
.then(response => {
  return response.json()
})
.then(data => {
  console.log(data)
})
```

We can even reduce this even further.

``` JavaScript
const requestUrl = 'http://ergast.com/api/f1/2008/5/results'

fetch(requestUrl)
.then(response => response.json())
.then(data => console.log(data))
```

The above technique uses `implicit returns`

Either way works exactly the same way. Choose which way works for you. Try find a way that has a good balance between readability and having the least amounts of code.

---

### Status Codes

The three most commonly see status codes are:

`200` means success

`404` means resources missing or not found.

`500` means that there is an internal server error.

If we do not receive a 200 status code, any user attemping to visit the web page can be redirected to a 404 page by adding the following code.

``` JavaScript
fetch(requestUrl)
.then(response => {
  if (response.status !== 200) {
    document.location.replace('./404.html')
  } else {
    return response.json()
  }
})
.then(data => {
  // do something with data here
})
```

***If the response status does not equal 200 then redirect user to the 404 page.***

---

### AJAX

AJAX is an important front-end web technology that lets JavaScript communicate with a web server. It lets you load new content without leaving the current page, creating a better, faster experience for your website's visitors.
**AJAX stands for Asynchronous JavaScript And XML**

XHR: short for XML HttpRequests.

Technically, AJAX's real name is called `XMLHttpRequest Object`.

Put simply, AJAX is the process of using JavaScript to send a request to a web server, and receive a response back, and then do something with that response. What you send to the web server with AJAX can be a simple request for a web page, a text file, a search sent to a database, or a complete form full of information.

You can send out multiple AJAX requests, and even though you send each request, one after another, you won't know which request will come back first. The speed of the server, the complexity of the request, and any internet traffic, all play a part in when a request returns information to the browser (client).

`The X in AJAX stands for XML or Extensible Markup Language.` XML also appears in the offficial name for this technology, XMLHttpRequest Object.

Originally, XML was seen as the format server responses should be sent in. It is not the most common and modern way of doing it.

#### How AJAX Works

1. Create a XMLHTTP Request object.

2. Create a callback function. This is where you process the returned data and update the HTML.

3. Open a request.

4. Send the request

##### Step 1

Create an XMLHttpRequest object

`var xher = new XMLHttpRequest()`

*This tells the web browser to get ready to work with AJAX and it is required anytime you would like to use AJAX.*

Note: you can call the variable anything you like. It is arbitrary.

In fact, for each AJAX request you should create a new XHR object.
For example, if you wanted to use AJAX twice on a page to request data, for a form submission, a sidebar and another submission form. You will need three variables each with the own XHR object.

##### Step 2

Create a callback function
This is the most complicated part of the AJAX process.
That is because the callback is the programming the browser to run when the server gets back with its response.
The callback function is the heart of your AJAX program, all the fun stuff you can think to do with the web server's response. Think of the callback as a note you leave the browser. Give me a call when you're ready
When the web browser sends off its AJAX request, it continues doing other things. This is the asynchronous part of AJAX. When the browser sends off an asynchronous request it doesnt just wait till it gets a response. If it did the browser would just freeze.
But, when the browser finally gets that response from the web server, it looks for that note, your callback, and gives it a call, and executing all of that programming you set up inside that callback.

There is another strange thing about AJAX. If you make multiple AJAX requests, you'll never know which request the server will respond back to first. In other words, you can never tell in which order your AJAX callbacks will run.

AJAX comes with its own set of events. We can add programming to respond to those events. The most important is the `.onreadystatechange` event.
This event is triggered whenever there's a change in a AJAX request.
Like opening a new request, sending it, or receiving a response. We create our callback to respond to that request.

``` JavaScript
xhr.onreadystatechange = function () {

}
```

This programming runs each time there is a change in state of the AJAX request. Each step in the AJAX process, like opening a new request or sending out that request triggers a change of state. In this callback function we are only interested in the final change of state. That is when the server sends back its response. We want to get that response and update our web page. The XMLHttpRequest object keeps track of the state using a special property named `.readystate`.
That property contains a number including the current state of the request and that propery holds the number `4`. When the `.readystate` property holds the number `4`, the request is done and the server has sent back a response.
Let's add a conditional statement to test for that state.

``` JavaScript
xhr.onreadystatechage = function() {
  if (xhr.readystate === 4) {
    document.querySelector('#ajax').innerHTML = xhr.responseText
  }
}
```

So here, we're checking if the ready state is equal to 4. That means we have got the response back. One we have the response back, we can do things like place the HTML data from the server into our document. Say we have a `<div id="ajax">`
we can select that using normal DOM manipulation methods and replace the innerHTML. Every XMLHttpRequest object has a property called `.responseText`.

The `.responseText` is the information that the web server sends back. Above we are taking the .`responseText` and storing it inside of the `div` with the `id="ajax"`.
In this case we have a simple callback. Remeber the programming doesn't run until the response comes back from the server. In fact, we have two more steps to complete the AJAX request.

##### Step 3

Open a request

An XHR object has a method or function called open.

``` JavaScript
var xhr = new XMLHttpRequest()

xhr.onreadystatechange = function () {
  if (xhr.readystate === 4) {
    document.querySelector('#ajax').innerHTML = responseText
  }
}
xhr.open('GET', 'sidebar.html')

```

The `.open()` function prepares the browser for sending the request.
You give the function TWO pieces of information. Also known as taking two parameters. The first is the HTTP method that you're going to use. The most common methods are GET and POST. But there are others, such as PUT and DELETE. You will use GET if you want to send a request for data. And POST if you are sending the data. Like information from a form, for the server to save in the database. The URL is where the request is going.
This could point to a file or a server-side program on your web server. With this example, it is just pointing to a file in the workspace. We'll load that file into the page. The `open()` just makes the browser ready to make the request, but it doesn't send that request. That is the last step of the process.

##### Step 4

Sending the request

``` JavaScript
var xhr = new XMLHttpRequest()
xhr.onreadystatechange = function () {
  if (xhr.readystate === 4) {
    document.querySelector('#ajax').innerHTML = responseText
  }
}
xhr.open('GET', 'sidebar.html')
xhr.send()
```

The previous three steps gives the browser all the information it needs. So we can finally send off the request to the web server.
Sending off the request takes just a simple bit of code.

`xhr.send()`

In our case since we're requesting a chunk of HTML, we don't provide any additional information in the send() function. But when you need to submit information to the server like the user's input from a web form,
you can pass the send() method that data.

Key Points
There are two common methods for sending HTTP requests:

- GET. Used for most requests. Browser uses the GET method whenever it requests a new web page, CSS file, image, and so on. Use GET when you want to "get" something from the server.

- POST. Used frequently with web forms to send data to store in a database. Use POST when sending data that will store, delete or update information from a database.

## Day 25

### Node.js

Node.js is a JavaScript runtime environment built on Google's Chrome V8 JavaScript engine. The runtime environment is designed to run outside of the browser, allowing developers to use JavaScript on the backend of their applications.

Ryan Dahl developed it in 2009, and its lastest iteration, version 18.16.0, was released in 2023. Developers use Node.js to create server-side web applications, and it is perfect for data-intensive applications since it uses an asynchronous, event-driven model.

#### Why do we use Node.js

There are many reasons for which Node.js is preferred for the server side of applications:

- NodeJs is built on Google's Chrome V8 engine, and for this reason its execution time is very fast and it runs very quickly.

- There are more than 50,000 bundles available in the Node Package Manager NPM and for that reason developers can import any of the packages any time according to their needed functionality for which a lot of time is saved.

- As NodeJs don not need to wait for an API to return data, so for building real time and data intensive web applications, it is very useful. It is totally asynchronous in nature that means it is totally non-blocking.

- The loading time for an audio or video is reduced by NOdeJs because there is better synchronization of the code between the client and server for having same code base.

- As NodeJs is open-source and it is nothing but a JavaScript framework, so for the developers who are already used to JavaScript, for them starting developing their projects with NodeJs is very easy.

### Arrow Functions

Arrow functions are pretty cool - they help you make code shorter and give less room for errors to hide. Because of this, they've become really popularr with experienced developers.

The basic syntax:
An arrow function is denoted by the fat arrow `=>`.

Here's what it looks like:

``` JavaScript
const arrowFunction = (arg1, arg2) => {
  // do stuff here...
}
```

If the function only requires one argument, it can be written without any paranthesises used around the argument. This is optional.

``` JavaScript
const arrowFunction = arg1 => {
  // do stuff here...
}
```

If there is only one line of code to be executed within the function, the function can be written all on one line like below examples with an **implicit return**.

``` JavaScript
const arrowFunction = arg1 => console.log('Hello, World!')
const arrowFunction = (arg1) => console.log('Hello, World!')
const arrowFunction = (arg1, arg2, arg3) => console.log('Hello, World!')
```

#### What is an explicit return

An explicit return is when you explicitly write return in the function.

``` JavaScript
const arrowFunction = arg => {
  return sum = arg * 2
}

console.log(arrowFunction(10))
// 20
```

Arrow functions are simply just anonymous functions. They become simple to understand once you place them side by side with a function expression.

``` JavaScript
// Arrow Function
const arrowFunction = (arg1, arg2) => {
  return sum = arg1 + arg2
}

// Function Expression
const normalFunction = function (arg1, arg2) {
  return sum = arg1 + arg2
}
```

There are two basic differences when converting a function expression to an arrow function.

- You remove the `function` keyword from a function expression

- You add a `=>` after `()` and before `{}`

#### Advanced Arrow Function Syntax

If the arrow function has zero parameters, you can replace the parenthesis with an underscore `_`.

``` JavaScript
const arrowFunction = _ => console.log('Hello, World!')
```

### `this` Keyword 5 Binding Rules

In JavaScript, the `this` keyword allows us to:

- Reuse functions in different execution context. It means, a function once defined can be invoked for different objects using `this` keyword.

- Identifying the object in the current execution context when we invoke a method.

#### Rule #1 How JavaScript Implicit Binding Works

Implicit binding covers most of the use-cases for dealing with the `this` keyword.

When we invoke a method of an object, we use the dot(.) notation to access it. In implicit binding, you need to check the object adjacent to the method at the invocation time. This determines what `this` is binding to.

Here is an example:

``` JavaScript
  const personDetails = {
    name: 'Matthew',
    address: '21535 Seven Hills Road, Vankleek Hill',
    message: function () {
      console.log(`${this.name} lives at ${this.address}`),
    }
  }

  personDetails.message()
  // Matthew lives at 21535 Seven Hills Road ....
```

  Here `this` is bound to the personDetails object. We know this because we invoke the method message() on the personDetails object. So `this.name` is going to log `Matthew` and `this.address` is going to log `21535 Seven Hills Road...`

Another Example

``` JavaScript
function greeting(obj) {
	obj.message = function () {
		console.log(`${this.name}! ${this.greeting}`)
	}
}

const matthew = {
	name: 'Matthew',
	greeting: 'How are you?',
}

const amy = {
	name: 'Amy',
	greeting: 'Sup! How are things?',
}

greeting(amy)
greeting(matthew)
matthew.message()
amy.message()

// Matthew! How are you?
// Amy! Sup! How are things?
```

## Day 29

### Object Oriented Programming

Object oriented programming is a style of writing JavaScript that uses Objects.
We use Object Oriented Programming when we want three things:

1. We want to create `instances` of objects
2. We want to extend objects via `Inheritance`
3. We want to hide properties via `Encapsulation`

#### Creating Instances of Objects

Below is a `blueprint` that spits out firtsName, lastName, age, and sex. We can send data to the blueprint  to create as many objects as we need. Objects created from blueprints are called `instances`.

``` JavaScript
function Person (firstname, lastName, age, sex) {
  this.firstName = firstName
  this.lastName = lastName
  this.age = age
  this.sex = sex
}
```

#### Creating a constructor

A constructor is a function. We begin constructors with a capital letter so we know it's different from normal functions.

In this case, let's call th constructor `Person`.

``` JavaScript
function Person() {
  // ...
}
```

We can use the `this` keyword inside a constructor to create properties. The `this` keyword refers to the instance that's going to be created later.

``` JavaScript
function House(bedrooms, bathrooms, garden, garage, ensuite) {
  this.bedrooms = bedrooms
  this.bathrooms = bathrooms
  this.garden = garden
  this.garage = garage
  this.ensuite = ensuite
}

  const myHouse = new House(5, 2, true, true, true)
  console.log(myHouse)

  // House {
//bedrooms: 5,
//bathrooms: 2,
//garden: true,
//garage: true,
//ensuite: true
//}
```

#### Creating an instance

You create an instance by doing two things:

1. Use the `new` keyword
2. Call the constructor function

`const myHouse = new House(5, 2, true, true)`

You can create as many instances as you want. Each instance will retain their individuality.

#### Instances in the wild

I have already been creating instances without knowing it.

For example, you create an array with `[]`, you actually create a new instance of `Array`. JavaScript simply lets you use `[]` as a shorthand to `new Array()`

``` JavaScript
const array = ['Matthew']
const array2 = new Array('Matthew')
```

The same applies to Objects. You've been creating Objects with `{}`. But JavaScript uses `new Object()` behind the scenes.

``` JavaScript
const object = {bedrooms: 4, bathrooms: 2, garage: false, garden: true} 
const object2 = new Object()
object2.bedrooms = 4
object2.bathrooms = 4
object2.garage = 4
object2.garden = 4
```

#### Creating a method in the constructor

``` JavaScript
function House(bedrooms, bathrooms, garden, garage, ensuite) {
	this.bedrooms = bedrooms
	this.bathrooms = bathrooms
	this.garden = garden
	this.garage = garage
	this.ensuite = ensuite
	this.printDetails = function () {
		let garden = ''
		let garage = ''
		let ensuite = ''
		this.garden ? (garden = 'does') : (garden = "doesn't")
		this.garage ? (garage = 'a') : (garden = 'no')
		this.ensuite ? (ensuite = 'a') : (ensuite = 'no')
		return `This house has ${this.bedrooms} bedrooms, ${this.bathrooms} bathrooms. It ${garden} have a garden. There is ${garage} garage and there is ${ensuite} ensuite.`
	}
}
const house1 = new House(3, 2, true, false, true)
const details = house1.printDetails()
// This house has 3 bedrooms, 2 bathrooms. It no have a garden. There is  garage and there is a ensuite.
```

### Four Flavours of Object Oriented Programming

There are four ways to create a blueprint fro Object Oriented Programming:

1. Constructor Syntax
2. Classes Syntax
3. OLOO
4. Factory Functions

#### Class Syntax

We can create a `class` with the `class` keyword. Like constructors, we begin th class with a capital letter.

It looks like this:

``` JavaScript
class House {
  constructor() {
    // code to initialize instances
  }
}
```

Everything that goes into a `Constructor` function would go into a class's  `constructor` method.

If you want to create a `Human` class with a `firstName` and `lastName` property, you'll write it like this:

``` JavaScript
class Human {
  constructor(firstName, lastName) {
    this.firstName = firstName
    this.lastName = lastName
  }
}


// Create a new instance
const person1 = new Human('Matthew', 'Millard)
console.log(person1)
// { firstName: 'Matthew', lastName: 'Millard' }
```

### Constructors vs Classes

**Constructor and class are the same thing.** Behind the scenes, JavaScript converts Classes into Contructors. That's why people say classes are **syntactic sugars**.

Even though `Constructors` look easier to use now (since there's less code), `Classes` become easier to use when `Inheritance` comes into play.

### OLOO Syntax

OLOO is an acronym for **Ojects Linking to Other Objects**.

The OLOO Syntaxt uses a JavaScript object as the blueprint. The mose basic form of an OLLO syntax is an empty object:

``` JavaScript
const OLOO = {
  // ...
}
```

You need a method inside the blueprint to initialise instances. This method is often called `init`. But it can also be called `constructor` `start`, or whatever you want.

In `init` you would write the same code as if you were writing the Constructor syntax.

``` JavaScript
const Human {
  init(firstName, lastName) {
    this.firstName = firstName
    this.lastName = lastName
  }
}
```

In `init` you would write the same code as if you were writing the Constructor syntax.

You create an instance with `Object.create`. This instance must then be initialized with the `init` function.

``` JavaScript

const Human {
  init(firstName, lastName) {
    this.firstName = firstName
    this.lastName = lastName
    return this
  }
}

const person1 = Object.create(Human)
person1.init('Matthew', 'Millard')
console.log(person1)
```

``` JavaScript
// More OLOO Object Linked to Other Object

const car = {
	init(brand, model, type, year, color) {
		this.brand = brand
		this.model = model
		this.type = type
		this.year = year
		this.color = color
		return this
	},
}

const vwTiguan = Object.create(car).init('Volkswagen', 'Tiguan', 'SUV', '2018', 'Black')
console.log(vwTiguan)

```

If you return `this` inside `init`, you can chain `Object.create` with the `init` method.

### Factory Functions

A Factory Function is a function that:

1. Returns an object
2. The returned object doesn't need the `new` keyword

The simplest factory function looks like this:

``` JavaScript
// Factory that returns an empty object
function Factory() {
  return {}
}
```

We can create the same `Human` blueprint by writing this:

``` JavaScript
// Creating a Factory
function Human(firstName, lastName) {
  return {
    firstName: firstName,
    lastName: lastName,
  }
}

const matthew = Human('Matthew', 'Millard')
console.log(matthew)
// 
```

You run the Factory Function to initialize the instance. (You don't need the `new`. You don't need to call `init` either.)

``` JavaScript
function House(bedrooms, bathrooms, garden, garage, type) {
	return {
		bedrooms: bedrooms,
		bathrooms: bathrooms,
		garden: garden,
		garage: garage,
		type: type,
	}
}

const newHouse = House(4, 2, true, true, 'detached')
console.log(newHouse)
// {
// bedrooms: 4,
// bathrooms: 2,
// garden: true,
// garage: true,
// type: 'detached'
// }
```

### Inheritance

Inheritance is a loaded word in Object Oriented Programming. Programmers use it to mean different things.

To understand Inheritance, we need to define this word into its fundamental form.

#### What is Inheritance?

Inheritance (in real life) is about getting stuff (like money and genes) from you parents.

**Inheritance** (in JavaScript) `is about getting properties` (**and methods**) `from parent objects`.

There are two ways to inherit properties:

1. Copy-Pasta
2. Delegation through Prototypes

#### Copy Pasta (Pasting)

Copy-pasting means you copy properties into the instance.
When you copy-paste, each instance will have its own version of the property.

Example: Let's say you want to create a `Human` constructor again.

``` JavaScript
function Human(firstName, lastName) {
	// Properties
	this.firstName = firstName
	this.lastName = lastName

	// Methods
	this.printName = function () {
		return `${this.firstName} ${this.lastName}`
	}
}

const newPerson = new Human('Matthew', 'Millard')
console.log(newPerson)
```

- Each Human has a firstName and lastName.

- Each `Human` should also be able to say their names with a method called `sayName`.

You can create an instance with the `new` keyword. Each instance will have its own properties. Properties are completely different from other instances.

``` JavaScript
const amy = new Human('Amy', 'Crooks')
const ginette = new Human('Ginette', 'Crooks')
const donald = new Human('Donald', 'Crooks')

```

Properties do not reference each other. If you change amy's printName method, it does not affect ginette's or donald's printName method.

``` JavaScript
function Human(firstName, lastName) {
  // Properties
  this.firstName = firstName
  this.lastName = lastName
  // Methods
  this.printName = function () {
    return `${this.firstName} ${this.lastName}`
  }
}

const amy = new Human('Amy', 'Crooks')
const ginette = new Human('Ginette', 'Crooks')
const donald = new Human('Donald', 'Crooks')

amy.printName = function() {
  return `${this.firstName}'s printName method will now be different from Ginette's and Donald's printName method.`
}

console.log(amy.printName());
// Amy's printName method will now be different from Ginette's and Donald's printName method.

```

### Delegation via Prototypes

When you delegate a task to another person (in real life), you ask that person to do the job for you.

When you delegate (in JavaScript), you ask the delegated object to call the property (or method).

Other names for Delegation via Prototype include:

1. Prototypal Inheritance
2. Prototype Inheritance
3. Prototypal Delegation
4. Prototype Delegation

All are interchangeable.

Example:

Each instance needs its own firstName and lastName properties.
We'll use the Copy-pasting method to create these two properties.

``` JavaScript
function Human(firstName, middleName, lastName) {
	this.firstName = firstName
	this.middleName = middleName
	this.lastName = lastName
	// We won't add any methods this time.
}
```

We can create it outside of the Human constructor, inside a prototype object. (All constructors have a prototype object.)

``` JavaScript
Human.prototype.printName = function () {
	return `${this.firstName} ${this.middleName} ${this.lastName}`
}
```

You can then create instances with the new keyword as before:

``` JavaScript
const matthew = new Human('Matthew', 'Richie', 'Millard')

// Human {
//firstName: 'Matthew',
//middleName: 'Millard',
//lastName: undefined
//}
```

As you can see, the matthew instance does not contain the printName method.

But they can both say their own names.

``` JavaScript
console.log(matthew.printName())
// Matthew Richie Millard
```

Instances can say their names because printName is declared inside the contructor's prototype. If you expand the `__proto__` object, you will see printName.

### The Prototype Chain

Here's what JavaScript does when you access a property:

**Step 1:** JavaScript checks if the property is available inside the object. If yes, JavaScript uses the property straight away.

**Step 2:** If the property is NOT inside the object, JavaScript checks if there's a Prototype available. If there is a Prototype, repeat Step 1 (and check if the property is inside the prototype).

**Step 3:** If there are no more Prototypes left, and JavaScript cannot find the property, it does the following:

- Returns undefined (if you tried to access a property).

- Throws an error (if you tried to call a method).

``` JavaScript
// Prototype Chain

function Car(brand, type, model) {
	this.brand = brand
	this.type = type
	this.model = model
}

// Create an instance of Car
const car1 = new Car('Volkswagen', 'SUV', 'Tiguan')
const car2 = new Car('Jeep', 'SUV', 'Compass')

// Add a method to the prototype object of the Car constructor object
Car.prototype.printCar = function () {
	return `${this.brand} ${this.model} is an ${this.type}`
}

// Add a property to the prototype object of the Car constructor object
Car.prototype.condition = 'Pre-owned'

console.log(car1.condition)
// Pre-owned
```

### The meaning of delegation

If a property is found inside a prototype, JavaScript asks the prototype for the property.

Each instance effectively hands over the job of accessing the property (or calling the method) to the prototype. In other words, they delegate the job away to the prototype.

Hence, the phrase Delegation via Prototype.

## Prototypal Delegation in 4 flavours

### Constructor Syntax

``` JavaScript
// Constructor Syntax - Add a method to the prototype object.

function Car(brand, model, year) {
	this.brand = brand
	this.model = model
	this.year = year
}

Car.prototype.printCar = function () {
	return `${this.brand} ${this.model} ${this.year}`
}

const newCar = new Car('VW', 'Tiguan', '2018')
console.log(newCar.printCar())
```

### Class Syntax

Prototypal Delegation is easier in Classes compared to constructors. You can write the property directly inside the class.

``` JavaScript
// Class Syntax - Add a method to the prototype

class CreateCar {
	constructor(brand, model, year) {
		this.brand = brand
		this.model = model
		this.year = year
	}
	// This adds the method printCar to the prototype object
	printCar() {
		return `${this.brand} ${this.model} ${this.year}`
	}
}

// Create an instance of a car
const car1 = new CreateCar('Jeep', 'Compass', '2016')
console.log(car1)

// Print the car details using the method in the prototype object
console.log(car1.printCar());
```

NOTE: Pay attention to the differences in syntax between classes and objects. This is one common mistake for developers who're new to the `class` syntax.

- Properties in classes are NOT seperated with `,`.

- Properties in objects ARE seperated with `,`.

### OLOO Objects Linking to Other Objects

``` JavaScript
const Car = {
	init(brand, model, year) {
		this.brand = brand
		this.model = model
		this.year = year
		return this
	},

	// Similiar to classes you can add a method or property to the prototype within side the constructor.
	printCar() {
		return `${this.brand} ${this.model} ${this.year}`
	},
}

// Notice that the init constructor object and printCar method are seperated by a comma.

// Create an instance using the OLOO syntax
const vehicle = Object.create(Car).init('VW', 'Tiguan', '2018')
console.log(vehicle)

// Call the printCar method
console.log(vehicle.printCar())
```

## Day 30

### Destructuring

If you want to get a value from an object, you need declare the variable and assign the value to it.

``` JavaScript
// Getting values from objects
const object = {
  car: 'Ferrari',
  house: 'Penthouse Suite',
  pet: 'dog',
}

const car = object.car
const house = object.house
const pet = object.pet
```

However, since the release of ES6, you can destructure variables - a process to declare and assign multiple variables with one line of code.

#### Destructuring Arrays

To destructure an array, you write the names of the variables you'd like to declare within square brackets(`[]`)

``` JavaScript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

const [first, second, third] = numbers

console.log(first, second, third) // 1 2 3
```

The first destructured variable will always be the first item in the array, the second destructured variable will always be the second item, and so on...

If there are not enough items in the array, the destructured variable will remain `undefined`.

#### Destructuring Objects

To destructure an object, you write the names of the properties you'd like to declare as variables in curly braces (`{}`).

``` JavaScript
// Destructuring an object

const person = {
	fName: 'Matthew',
	lName: 'Millard',
	age: 34,
	pets: {
		dog: 2,
		cat: 1,
	},
}

const { fName, lName, age, pets } = person
console.log(fName, lName, age, pets.dog, pets.cat)
```

If you try to destructure a non-existant property, you'll get `undefined`.

``` JavaScript
const person = {
  name: 'Matthew',
  age: 34,
  gender: 'Male',
}

const { sexuality } = person
console.log(sexuality)
// undefined
```

### Destructuring with a different variable

You declare variables when you destructure. That means you cannot have two variables of the same name. For example, say you had a variable declared in the global scope, and you defined a variable in the destructuring of the object or array with a matching name, it would throw and error.

However, you can change the name of your destructured variable with colon (`:`).

### Destructuring function arguments

You can also destructure function arguments if the arguments is an array or an object.

``` JavaScript
// Object Example

const person = {
	fName: 'Matthew',
	lName: 'Millard',
	age: 34,
	pets: {
		dog: 2,
		cat: 1,
	},
}

function printDetails({ fName, lName, age, pets }) {
	console.log(`My name is ${fName} ${lName}, I am ${age} years old and I have ${pets.dog} dogs and ${pets.cat} cat.`)
}

printDetails(person)
// My name is Matthew Millard, I am 34 years old and I have 2 dogs and 1 cat.
```
#### Destructuring as an argument - Array

``` JavaScript
// Destructuring Arrays as an argument

const people = ['Matthew', 'Amy', 'Ginette', 'Donald']

function getPerson([person1, person2, person3, person4]) {
	switch ('Donald') {
		case person1:
			console.log(`Person1 is Donald.`)
			break
		case person2:
			console.log(`Person2 is Donald.`)
			break
		case person3:
			console.log(`Person3 is Donald.`)
			break
		case person4:
			console.log(`Person4 is Donald.`)
			break
		default:
			console.log('Donald is not in the array.')
			break
	}
}

getPerson(people)
// Person4 is Donald.
```

#### Default parameters when destructuring

You can provide fallback values for destructured variables with `=.

``` JavaScript
// Fallback value for destructured array
const people = ['Matthew', 'Gareth', 'Daniel', 'Garry', 'Suzi']

const [person1, person2, person3, person4, person5, person6 = 'Ella'] = people

console.log(person6)
// Ella
```
``` JavaScript
// Fallback value for destructured object
const course = { name: 'Learn JavaScript' }
const { description = 'Best JavaScript course ever!' } = course

console.log(description) // Best JavaScript course ever!
```

### Wrapping Up

Destructing gives you a way to extract values from objects and arrays quickly.

To destructure an array, you use `[]`. The first destructured variable is always the first item in the array, the second destructured variable is the second item in the array, and so on.

To destructure an object, you use `{}`. The destructured variable should be the property name of the object. You can even rename destructured variable if you wish too.

You can also provide default values to a destructured variable if it doesn't exist.

