## HTML5 interview questions.



### 1. Write a HTML table tag sequence that outputs the following

```html
    50 pcs 100 500
    10 pcs 5 50
```

Answer:

``` html
<table>
  <tr>
    <td>50 pcs</td>
    <td>100</td>
    <td>500</td>
  </tr>
  <tr>
    <td>10 pcs</td>
    <td>5</td>
    <td>50</td>
  </tr>
</table>
```

### 2. What is an iframe and how it works?

Answer: 

> An iframe is an HTML document which can be embedded inside another HTML page.

```html
<iframe src="https://github.com" height="300px" width="300px"></iframe>
```

### 3. Explain meta tags in HTML

Answer:

- Meta tags always go inside head tag of the HTML page
- Meta tags is always passed as name/value pairs
- Meta tags are not displayed on the page but intended for the browser
- Meta tags can contain information about character encoding, description, title of the document etc

Example:

```html
<!DOCTYPE html>
<html>
<head>
  <meta name="description" content="I am a web page with description"> 
  <title>Home Page</title>
</head>
<body>
  
</body>
</html>
```

### 4. What is the purpose of the alt attribute on images?

Answer:

> The alt attribute provides alternative information for an image if a user cannot view it. The alt attribute should be used to describe any images except those which only serve a decorative purposes, in which case it should be left empty.

### 5. What is the difference between span and div?

Answer:

- **div** is a block element
- **span** is inline element

> For bonus points, you could point out that it’s illegal to place a block element inside an inline element, and that while div can have a p tag, and a p tag can have a span, it is not possible for span to have a div or p tag inside.

### 6. How can you highlight text in HTML?

Answer: 

> If you are working with an HTML5 page, the `<mark>` tag can be a quick and easy way of highlighting or marking text on a page:

```html
    <mark>highlighted text</mark>
```

> To highlight text with just HTML code and support for all browsers, set the background-color style, as shown in the example below, using the HTML tag.


```html
    <span style="background-color: #FFFF00">Yellow text.</span>
```

### 7. What were some of the key goals and motivations for the HTML5 specification?

Answer:

> HTML5 was designed to replace HTML 4, XHTML, and the HTML DOM Level 2. The key goals and motivations behind the HTML5 specification were to:

- Deliver rich content (graphics, movies, etc.) without the need for additional plugins, such as Flash.
- Provide better semantic support for web page structure through new structural element tags.
- Provide a stricter parsing standard to simplify error handling, ensure more consistent cross-browser behaviour, and simplify compatibility with documents written to older standards.
- Provide better cross-platform support whether running on a PC, Tablet, or Smartphone.

### 8. What is Character Encoding?

Answer:

> To display an HTML page correctly, a web browser must know which character set (character encoding) to use. This is specified in the tag:

HTML 4:

```html
  <meta http-equiv="Content-Type" content="text/html;charset=ISO-8859-1">
```

HTML5: 

```html
  <meta charset="UTF-8">
```

### 9. What is a self closing tag?

Answer:

> In HTML5 it is not strictly necessary to close certain HTML tags. The tags that aren’t required to have specific closing tags are called “self closing” tags.

> An example of a self closing tag is something like a line break (`<br />`) or the meta tag (`<meta>`). This means that the following are both acceptable:

```html
  <meta charset="UTF-8">
  ...
  <meta charset="UTF-8" />
```

### 10. How Can I Get Indexed Better by Search Engines?

Answer:

> It is possible to get indexed better by placing the following two statements in the `<HEAD>` part of your documents:

```html
  <META NAME="keywords" CONTENT="keyword keyword keyword keyword">
  <META NAME="description" CONTENT="description of your site">
```
Both may contain up to 1022 characters. If a keyword is used more than 7 times, the keywords tag will be ignored altogether. Also, you cannot put markup (other than entities) in the description or keywords list.

### 11. Briefly describe the correct usage of the following HTML5 semantic elements: header, article, section, footer

Answer:

> `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author’s name, time and date of publication, table of contents, or other navigational information.

> `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing it’s meaining. Individual blog posts or news stories are good examples.

> `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

> `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author’s name, copyright information, and related links are typical examples of such content.

### 12. What's the difference between an "attribute" and a "property" in HTML?

Answer:

> Attributes are defined on the HTML markup but properties are defined on the DOM. To illustrate the difference, imagine we have this text field in our HTML:

``` javascript
<input type="text" value="Hello">.

const input = document.querySelector('input');
console.log(input.getAttribute('value')); // Hello
console.log(input.value); // Hello
```
>But after you change the value of the text field by adding "World!" to it, this becomes:

```javascript
console.log(input.getAttribute('value')); // Hello
console.log(input.value); // Hello World!
```
Source: https://devinterview.io/dev/html5-interview-questions