# Front-End-Interview-Questions

### 1) What is the DOM in HTML?
* The Document Object Model (DOM) is a programming interface for HTML documents. It represents the page so that programs can change the document structure, style, and content.The DOM represents the document as nodes and objects.

### 2) What is the difference between span and div?
* span is an inline element
* div is a block element
* Divs should be used to wrap sections of a document, while spans should be used to wrap small portions of text, images, etc.
* Bonus point, it is illegal to place a block-level element within an inline element.

```jsx
Example:
 <div>Hi<span>I'm the start of the span element <div>I'm illegal</div> I'm the end of the span</span> Bye I'm the end of the div</div>
```
### 2) What are Meta Tags?
Meta tags are snippets of text that describe a page’s content; the meta tags don’t appear on the page itself, but only in the page’s source code.
Meta tags are essentially little content descriptors that help tell search engines what a web page is about.

```jsx
Examples:
<head>
  <meta charset="UTF-8">
  <meta name="description" content="Description search engines use">
  <meta name="keywords" content="Keywords, of, your, page">
  <meta name="author" content="Me">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### 3) What is the difference between an ID selector and the Class selector in CSS?
* IDs are unique. Each element can have only one ID and the HTML page can only have one element with that ID
* Classes are not unique. You can use the same class on multiple elements and an element can have many classes.
* Any styling information that needs to be applied to multiple objects on a page should be done with a class.

### 4) How could you apply CSS rules specific to a media?
* The @media rule is used in media queries to apply different styles for different media types/devices.
```jsx
Example:
/* Change the background color of the any <div> element to "red" when the browser window is 600px wide or less */
@media only screen and (max-width: 600px) {
  div {
    background-color: red;
  }
}
```
