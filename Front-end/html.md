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

Source: https://devinterview.io/dev/html5-interview-questions