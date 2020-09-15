# Front-End-Interview-Questions

### 1) What is the DOM in HTML?
The Document Object Model (DOM) is a programming interface for HTML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects.

### 2) What is the difference between span and div?
span is an inline element
div is a block element
Divs should be used to wrap sections of a document, while spans should be used to wrap small portions of text, images, etc.
Bonus point, it is illegal to place a block-level element within an inline element.

```jsx
Example:
 <div>Hi<span>I'm the start of the span element <div>I'm illegal</div> I'm the end of the span</span> Bye I'm the end of the div</div>
```
