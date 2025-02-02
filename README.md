# swe_module2

# HTML Structure and Style 

Overview: Apprentices will learn more about HTML, with the session focusing on HTML structure and style. 

Objectives: 
<ul>
  <li>I will be able to create structure to a page using HTML elements </li>
  <li>I will be able to provide an example of determine vs indeterminate progress </li>
</ul>

Lets start with a good basis for our application by creating the HTML structure and style it using a responsive flexible css grid layout.

We are going to use semantic HTML elements. Semantics is the study of the meanings of words and phrases in a language. Semantic elements are elements with a meaning.

Look at the examples below.

```html
    <body>
        <div>
            <div>
                <a href="/">Home</a>
                <a href="/about">About</a>
                <a href="/shop">Shop</a>
            </div>
        </div>
        <div>
            <div>
                <div>
                    <img src="/images/slipper-01.jpg" alt="slipper 01" />
                    <div>£29.99</div>
                    <button>Add to Cart</button>
                </div>
                <div>
                    <img src="/images/slipper-02.jpg" alt="slipper 02" />
                    <div>£29.99</div>
                    <button>Add to Cart</button>
                </div>
                <div>
                    <img src="/images/slipper-03.jpg" alt="slipper 03" />
                    <div>£29.99</div>
                    <button>Add to Cart</button>
                </div>
            </div>
        </div>
        <div>
            <span>my slipper company</span>
        </div>
    </body>
```

Whilst this is valid HTML it does not have much meaning. By using the semantic elements we can layout our page structure in the same way, but also communicate to other programs that read our HTML how to treat the different areas. Those other programs might be, a search engine indexing our page, a screen reader, different browsers rendering out page. For example google uses the `<article>` elements to determine the subject of a page.

Let us have a look at the same layout but use semantic elements.

```html
    <body>
        <header>
            <nav>
                <a href="/">Home</a>
                <a href="/about">About</a>
                <a href="/shop">Shop</a>
            </nav>
        </header>
        <main>
            <section>
                <article>
                    <hgroup>
                        <h1>Slipper</h1>
                        <h2>Our most comfortable</h2>
                    </hgroup>
                    <figure>
                        <img src="/images/slipper-01.jpg" alt="slipper 01" />
                        <figcaption>£29.99</figcaption>
                    </figure>
                    <button>Add to Cart</button>
                </article>
            </section>
        </main>
        <footer>
            <span>my slipper company</span>
        </footer>
    </body>
```

|HTML elements|Description|
|:---|:---|
`<header>`|Defines the top of a section or page
`<main>`|Represents the dominant content of the of a document or component
`<footer>`|Defines the bottom of a section or page or component
`<article>`|Defines self-contained areas on a page
`<nav>`|Defines navigation to other pages in the site
`<hgroup>`|Defines a group of headings (H1–H6 elements) *this is now depreciated
`<figure>`|Defines content that contains a figure, such as an image, chart, or picture
`<figcaption>`|Defines the caption of a figure element


In addition to the elements above you should also know about and try to use the following:

|HTML elements|Description|
|:---|:---|
`<aside>`|Defines smaller content areas outside the flow of a webpage
`<mark>`|Defines text that should be highlighted
`<progress>`|Defines the progress of the task

## Using the `<hgroup>` element

The `<hgroup>` element is a semantic method that organises headers and sub-headers. This element typically contains the standard and familiar `<h1>` to `<h6>` elements. The `<hgroup>` element groups related headers in sequence.

## Test Your Knowledge

Can you answer the Kahoot question correctly? <a href="https://create.kahoot.it/share/8166da78-4e47-47a1-935a-72989717b649">Click on the link!</a>

## Using the `<progress>` element

The `<progress>` element represents the progress of an objective or task. The two supported types of progress tasks are **determinate** and **indeterminate**.

Use a **determinate** progress task when you know in advance the amount of work to be completed; in other words, you know the starting and ending values. Sample scenarios for this case include downloading a file for which you know the exact size or displaying the progress of a fundraising effort. In both situations, you know the exact status of the task at any particular time, and you also know what the end goal is—either the number of bytes for the file download or the number of dollars for the fundraiser. In these determinate cases, you can specify HTML5 markup such as this:

```html
    <p>Our goal is to have 1000 users:</p>
    <span>0</span>
    <progress value="50" max="1000"></progress>
    <span>1000</span>
```

<progress value="50" max="1000"></progress>

As shown in the preceding code, the `<progress>` element has two attributes you need to know: value and max. The value attribute lets you specify the current value or position of the `<progress>` element at a specific point in time. The max attribute tells the browser what the maximum possible value is for the element. The browser uses these two values to determine how much of the element should be coloured in. So if I change the value to 750 the progress bar displays the new value like this:

<progress value="750" max="1000"></progress>

You use **indeterminate** tasks when you don’t know how long a task will take to complete but still want to show users that some work is occurring and that they should wait. When you don’t specify the value attribute, the browser can infer that the `<progress>` element represents an indeterminate task.

<progress></progress>

Downloading...

Can you see the bar is subtly pulsing?

## Using the `<mark>` element

    Use the `<mark>` element to <mark>highlight</mark> text

Use the `<mark>` element to <mark>highlight</mark> text.

## Test Your Knowledge

Can you match the element to its description? <a href="https://www.educandy.com/site/resource.php?activity-code=3f130">Click on the link to test yourself!</a>

## Assignment 
You have now been introduced to the HTML elements you’ll need to know about for the exam. We can use these to layout our app’s page. Take some time to think about how you would want the music player app to look. Where will the text go? Other images? If you need to design in a notebook first feel free and annotate the drawing with pseudocode. 
