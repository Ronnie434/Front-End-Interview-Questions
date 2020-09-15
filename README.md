# Front-End-Interview-Questions

### 1) What is the DOM in HTML?
* The Document Object Model (DOM) is a programming interface for HTML documents. It represents the page so that programs can change the document structure, style, and content.The DOM represents the document as nodes and objects.

### 2) What is the difference between span and div?
* **span** is an inline element
* **div** is a block element
* Divs should be used to wrap sections of a document, while spans should be used to wrap small portions of text, images, etc.
* Bonus point, it is illegal to place a block-level element within an inline element.

```jsx
Example:
 <div>Hi<span>I'm the start of the span element <div>I'm illegal</div> I'm the end of the span</span> Bye I'm the end of the div</div>
```
### 2) What are Meta Tags?
* **Meta tags** are snippets of text that describe a page’s content; the meta tags don’t appear on the page itself, but only in the page’s source code.
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
* **IDs** are unique. Each element can have only one ID and the HTML page can only have one element with that ID
* **Classes** are not unique. You can use the same class on multiple elements and an element can have many classes.
* Any styling information that needs to be applied to multiple objects on a page should be done with a class.

### 4) How could you apply CSS rules specific to a media?
* The **@media** rule is used in media queries to apply different styles for different media types/devices.
```jsx
Example:
/* Change the background color of the any <div> element to "red" when the browser window is 600px wide or less */
@media only screen and (max-width: 600px) {
  div {
    background-color: red;
  }
}
```

### 5) In CSS what are Pseudo-classes?
* A Pseudo class in CSS is used to define the special state of an element. It can be combined with a CSS selector to add an effect to existing elements based on their states.
```jsx
Example(s):
/* 
   Any <a> element which the user's pointer is hovering will go green 
*/
a:hover {
  color: green;
}
/* Selects any <a> that has been visited and makes the text purple*/
a:visited {
  color: purple;
}
```
* **Bonus point** can they name any? It’s quite a big list https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes

### 6) What’s the difference between a relative, fixed, absolute and statically positioned element?
* **Relative** the element is positioned relative to its normal position.
* **Fixed** the element is positioned related to the browser window.
* **Absolute** the element is positioned absolutely to its first positioned parent.
* **Static** this is the default value, all elements are in order as they appear in the document.

### 7) What is the difference between PUT and POST?
* **PUT:** Replaces target resource with the request payload. Can be used to update or create a new resource.
* **POST:** Performs resource-specific processing on the payload. Can be used for different actions including creating a new resource, uploading a file or submitting a web form.
* **Bonus point:**
One other difference is that PUT should be idempotent — multiple PUTs of the same data to the same URL should be fine, whereas multiple POSTs might create multiple objects or whatever it is your POST action does.

### 8) What are the differences between Long-Polling, Websockets and Server-Sent Events?
* **Long-polling** opens an HTTP request and remains open until an update is received. Upon receiving an update, a new request is immediately opened awaiting the next update.
* **WebSockets** The WebSocket protocol allows for constant, bi-directional communication between the server and client. For this test, Primus is used to abstract multiple implementations of the protocol.
* **Server-sent events** rely on a long-lived HTTP connection, where updates are continuously sent to the client

### 9) Explain the difference between cookies, session storage, and local storage?
* **Local Storage** as it’s called its local storage for your browsers, it can save up to **10MB, Session Storage** does the same, but as its name saying, it’s session based and will be deleted after closing your browser. Sessions storage saves less up to 5mb.
* **Cookies** are very tiny data storing in your browser, that can save up **4KB** and can be accessed through server or browser both

### 10) What is CORS?
* **CORS** stands for Cross-Origin Resource Sharing.
* CORS is a browser mechanism which enables controlled access to resources located outside of a given domain. It extends and adds flexibility to the same-origin policy

### 11) What is a promise?
* They are used to handle asynchronous operations. They can handle multiple asynchronous operations easily and provide better error handling than callbacks and events.

### 12) What are the different states in promises?
* A Promise has three states:
**1) fulfilled:** Action related to the promise succeeded
**2) rejected:** Action related to the promise failed
**3) pending:** Promise is still pending i.e not fulfilled or rejected yet

### 13) What is Hoisting in JavaScript?
* **Hoisting** is the term used to describe the moving of variables and functions to the top of their (global or function) scope on where we define that variable or function.

### 14) What are the falsy values in JavaScript?
* **Falsy** values are values that when converted to boolean becomes false.
```
**Any of the below:**
'' 
0 
null
undefined
NaN
false
-0
On // BigInt, when used as a boolean, follows the same rule as a Number
```

## Conclusion:
* I’ve asked and been asked a mixture of the above questions in interviews. A combination of a coding challenge(s) with some quick-fire questions is a good way to see a candidates potential.
* I think for frontend developer interviews you will need more JavaScript questions than above. Below are some JavaScript & TypeScript questions.

