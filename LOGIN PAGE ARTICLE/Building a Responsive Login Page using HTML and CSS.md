![](https://github.com/lilyflowr/Technical-Writing/blob/main/LOGIN%20SCRN%20ARTICLE/responsive%20html%20and%20css%20login.gif)

# Building a Responsive Login Page using HTML and CSS
## Introduction:

Responsive web design provides an optimal experience for users across devices. As mobile and tablet usage grows, websites must dynamically adapt to any screen size.

This guide teaches beginners how to build a responsive login page with HTML and CSS. You will set up the HTML structure, style the page, add input fields and a button, and ensure the page works on all viewport sizes. Following the step-by-step instructions, even those new to web development can make a responsive login form.

## Prerequisites:
To get started, you should know some HTML and CSS basics. You'll also need a text editor and web browser.

## Setting up the HTML Structure
First, set up an HTML file to create a simple responsive login page. In the ```<head>```, define the page title, character set as UTF-8, and viewport. The viewport meta tag ensures the page is scaled properly on mobile devices.

```html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Login Page</title>
</head>
```

Next, add a ```<div>``` with the class "container" to center the content. Add a ```<h1>``` header and a ```<form>``` tag within the container.


``` html
<div class="container">
     <h1>Login</h1> 
     <form> 
        <!-- Input fields go here -->
    </form> 
</div>
```

## Styling the Page with CSS
Create a CSS file called index.css. Link the CSS file to the HTML by adding the following line within the ```<head>``` Tags:

```html
<link rel="stylesheet" href="index.css">
```
Style the body by setting the font family and background color and removing the margin and padding:

```css
  body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    margin: 0;
    padding: 0;
  }
```
For the container, set a max-width of 400px, center it with margin: auto, add a background color, padding, border radius for rounded corners, and a box shadow. Center the ```<h1>``` Header within the container and add the bottom margin:

```css
  .container {
    max-width: 400px;
    margin: 100px auto;
    background-color: #fff;
    padding: 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }

  .container h1 {
    text-align: center;
    margin-bottom: 20px;
  }
```

Style the input fields by setting the width to 100%, adding padding, margin-bottom, a border, border-radius, and box-sizing to account for the padding in width. Make the button 100% width, add padding, set the background and text colors, remove the border, and add a border radius and cursor: pointer.

```css
  .container input[type="text"],
  .container input[type="password"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border: 1px solid #ccc;
    border-radius: 3px;
    box-sizing: border-box;
  }

  .container button {
    width: 100%;
    padding: 10px;
    background-color: #4CAF50;
    color: #fff;
    border: none;
    border-radius: 3px;
    cursor: pointer;
  }
```

Use media queries to adjust the styling for mobile devices. For screens 480px and below, increase the container's top margin.

```css
  @media (max-width: 480px) {
    .container {
      margin-top: 50px;
    }
  }

```
## Adding Input Fields and a Button
Inside the ```<form>``` element, insert the following code to create the input fields and submit button:

```html
<input type="text" placeholder="Username" required> 
<input type="password" placeholder="Password" required> 
<button type="submit">Login</button>
```
## Testing the Page
Save the HTML and CSS files, then open the HTML in a browser to view the responsive login page. The page will have a centered form container with rounded corners, input fields, and a submit button. The container will shift up on mobile to account for the smaller screen size.

Congratulations, you built a responsive login page! You learned how to set up the HTML structure, style the page with CSS, add input fields and a button, and ensure the page is responsive. You can build on these skills by adding validation, connecting the form to a server, and experimenting with more advanced styling. Be sure to save backups of your work as you progress.

