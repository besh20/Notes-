# HTML Notes

**Html Tags**

1. Empahsis tag

```html
<em> Web tech </em>
```

1. Override The Current Text Direction tag

```html
<bdo> Web tech </bdo>
```

1. A section that is quoted from another source:

```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature. The world's 
leading conservation organization, WWF works in 100 countries and is supported 
 1.2 million members in the United States and close to 5 million globally.
</blockquote>
```

1. display a web page within a web page.

```html
<iframe src="url" title="description"></iframe>
```

1. contains several elements for defining user input and computer code.

```html
<code>
x = 5;
y = 6;
z = x + y;
</code>
```

1. File Path

| Path | Description |
| --- | --- |
| <img src="picture.jpg"> | The "picture.jpg" file is located in the same folder as the current page |
| <img src="images/picture.jpg"> | The "picture.jpg" file is located in the images folder in the current folder |
| <img src="/images/picture.jpg"> | The "picture.jpg" file is located in the images folder at the root of the current web |
| <img src ="../picture.jpg"> | The "picture.jpg" file is located in the folder one level up from the current folder |
1. defines a division or a section in an HTML document.

```html
<div class="myDiv">
  <h2>This is a heading in a div element</h2>
  <p>This is some text in a div element.</p>
</div>Html Form
```

1. link element 

```html
<a href="https://www.w3schools.com/">Visit W3Schools.com!</a>
```

1. img element

```html
<img src="pic_trulli.jpg" alt="Italian Trulli">
```

1. define a client side script 

```html
<script src = "script.js "></script>
```

1. define a container for a content that should be hidden when the page loads

```html
<template>
<h1>web tech</h1>
<h2>day 1</h2>
</template>
```

1. HTML ordered and unordered list

 

```html
<ol>
<li>tea</li>
<li>coffee</li>
<li>milk</li>
</ol>

<ul>
<li>tea</li>
<li>coffee</li>
<li>milk</li>
</ul>
```

1. Audio Tag

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio tag.
</audio>
```

1. Video Tag 

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
  Your browser does not support the video tag.
</video>
```

1. break line 

```html
<p>To force<br> line breaks<br> in a text,<br> use the br<br> element.</p>
```

B. HTML form 

1. element is used to create an HTML form for user input

```html
<form>
.
form elements
.
</form>
```

1. form input element

| Type | Description |
| --- | --- |
| <input type="text"> | Displays a single-line text input field |
| <input type="radio"> | Displays a radio button (for selecting one of many choices) |
| <input type="checkbox"> | Displays a checkbox (for selecting zero or more of many choices) |
| <input type="submit"> | Displays a submit button (for submitting the form) |
| <input type="button"> | Displays a clickable button |
1. text fields

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

1. The Action Attribute 

The `action` attribute defines the action to be performed when the form is submitted.

```html
<form action="/action_page.php">
```

1. The Method Attribute

The `method` attribute specifies the HTTP method to be used when submitting the form data.

The form-data can be sent as URL variables (with `method="get"`) or as HTTP post transaction (with `method="post"`).

The default HTTP method when submitting form data is GET.

```html
<form action="/action_page.php" method="get">
<form action="/action_page.php" method="post">
```

**Notes on GET:**

- Appends the form data to the URL, in name/value pairs
- NEVER use GET to send sensitive data! (the submitted form data is visible in the URL!)
- The length of a URL is limited (2048 characters)
- Useful for form submissions where a user wants to bookmark the result
- GET is good for non-secure data, like query strings in Google

**Notes on POST:**

- Appends the form data inside the body of the HTTP request (the submitted form data is not shown in the URL)
- POST has no size limitations, and can be used to send large amounts of data.
- Form submissions with POST cannot be bookmarked