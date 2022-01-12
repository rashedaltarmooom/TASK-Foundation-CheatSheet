# HTML Basics

HTML is a markup language. Everything you write in html should be wrapped in **Tags**. There are 2 main types of tags

1. Self closing tag. `_TAG __`
2. Non-self closing tag. `_TAG_ CONTENT __TAG_` And it contains 3 main parts
   1. **Opening Tag** `_TAG_`
   2. **Inner HTML**: The content that will be rendered between the opening and closing tag.
   3. **Closing Tag** `__Tag_`

## Attributes

Every tag can have **ATTRIBUTES**. Attributes are added to the the **opening tag only**.
Every attribute added would have a name, then `___` sign then the value of the attribute between quotations.

```html
<TAG ATTRIBUTE="VALUE"> CONTENT </TAG>
```

For example, the **style** attribute can be added to the following tag as follows

```html
<TAG ____="background-color: red;"> CONTENT </TAG>
```

## HTML structure

HTML has 2 main tags

1. `<___>` is a tag that we add meta data to it, like linking the CSS, or adding a title for a website. Anything inside this tag, shall not be rendered in the web page directly
2. `<___>` is a tag that we add the content of the html page that will be rendered directly to the web page

## Comments 💬

HTML comments are just comments and notes for the developers to understand the code structure, or sometimes intentionally hide some html block to not be rendered on the page.

```html
<____> MY COMMENTS HERE <____>
```

## Headings 📰

Headings are big titles. There are 6 sized of headings.

```html
  <___> This is heading 1</___>
  <___> This is heading 2</___>
  <___> This is heading 3</___>
  <___> This is heading 4</___>
  <___> This is heading 5</___>
  <___> This is heading 6</___>
```

## Paragraphs ❡

Paragraph creates a new line for a text body.
The following paragraphs will be rendered in two separate

```html
<___> This is a paragraph</___>
<___> This is another paragraph</___>
```

## Images 🌁

Images are self closing tags. They need 1 main attribute `___`, which needs the image link.

```html
<___ ___="IMAGE_LINK"/>
```

Note that the image link should be wrapped with quotation marks `" "`

Another attribute that the image takes is `___` which is an alternative text that would appear if the image link was broken, or couldn't be loaded. Also it's useful for screen readers to describe the image.

```html
<___ ___="IMAGE_LINK" ___="ALTERNATIVE_TEXT"/>
```

## Links - Anchor tag ⚓️

Anchor tag `<_>` is a **non-self closing tag**. The inner html of the anchor tag is the text that will be tapped to take you to a specific link. It takes one required attributes `___` that should take the link of the destination of the link.

```html
<_ ____="https://google.com"> CLICK ME </_>
```

You can specify if you want to open the tag within the same window or different window or different tab using the attribute `______`

```html
<!-- OPEN IN A NEW TAB -->
<a ______="_____" href="https://google.com"> CLICK ME </a>

<!-- OPEN IN A NEW WINDOW -->
<a ______="_____" href="https://google.com"> CLICK ME </a>
```

## Lists ❥

There are two types of lists. **ordered list**, and **unordered list**. For both lists, there will be list items.

### Ordered list

```
1. list item one
2. list item two
3. list item three
```

```html
<__>
   <__> list item one </__>
   <__> list item two </__>
   <__> list item three </__>
</__>
```

### Unordered list

```
- point
- point
- point
```

```html
<__>
  <__> point </__>
  <__> point </__>
  <__> point </__>
</__>
```

To change the ordered list type to show the list with alphabetical order or romanian as follows

```
A. Point 1
B. Point 2
C. Point 3

  I. Point 1
 II. Point 2
III. Point 3
```

We use the attribute `____`

```html
<!-- Alphabetical -->
<ol ____>
  <li>Point 1</li>
  <li>Point 2</li>
  <li>Point 3</li>
</ol>
<!-- Romanian -->
<ol ____>
  <li>Point 1</li>
  <li>Point 2</li>
  <li>Point 3</li>
</ol>
```

## Head main tags 🧠

`<head>` tag contains the meta data of the page. Here are the most used ones:

### Changing the title of the web page

```html
  <head>
    <___> I am title </___>
  </head>
```

### Linking a css file

```html
<head>
  <___________ />
</head>
```
