# Coding Bootcamp Daily Notes

## Table of Contents

- [Day 01](#Day-01)
  - [Computaional Thinking](#Computational-Thinking)
  - [Git & Command Line](#Git-&-Command-Line)
  - [User Story & Acceptance Criteria](#User-Story-&-Acceptance-Criteria)
- [Day 02](#Day-02)
  - [Set Up a Local Repository](#Local-Repository)
  - [HTML Attributes](#HTML-Attributes)
- [Day 03](#Day-03)
  - [CSS Visibility vs Display Property](#CSS-Properties)


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


### Git & Command Line

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

### User Story & Acceptance Criteria

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

## Day 02

### Set Up a Local Repository

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

## Day 03

### CSS Visibility vs Display Property

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
- inline-block: it sets the element to a block box inside an inline box. This is required often to change an inline element into a inline-block so you can apply margins and padding.

Simply put, `display: none;` completely gets rid of the tag, as it had never existed in the HTML page whereas `visibility: hidden;` just makes the tag invisible, it will still sit on the HTML page occupying space, it's just invisible.




