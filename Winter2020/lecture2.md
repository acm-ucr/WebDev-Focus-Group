# Web Dev Focus Group - Personal Site workshop (cont.)

Today, we'll improve your personal website project by showing you how to add

1. Multiple pages and a cool nav bar
2. A contact page with a form that emails you 
3. Cool fonts
4. A header tag with info like a site icon
5. Basic mobile responsiveness


## 1 - Adding a nav bar, linking other pages

Building a cool nav bar is pretty simple. First, create the pages you want your users to visit. Then, we use an unordered list and use some css rules to remove the bullet points and make it show up horizontally


HTML:

```
 <ul>
  <li><a href="index.html">Home</a></li>
  <li><a href="contact.html">Contact</a></li>
  <li><a href="about.html">About</a></li>
</ul> 
```


CSS:

```
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  overflow: hidden;
}

li {
  float: left;
}

li a {
  display: block;
  padding: 8px;
  background-color: #dddddd;
}
```
[source](https://www.w3schools.com/css/css_navbar.asp)

Get creative with the colors and other attributes to make something that reflects you!

## Adding formspree

1. Make an account at [formspree.io](https://formspree.io/)
2. Create a new form with the desired fields and paste the html into your new contact page

It's that easy!

## Adding fonts

1. Head over to [google fonts](https://fonts.google.com/)
2. Choose a font and grab the `<link>` tag, and put it in your header, eg.
```
<head>
 <link href="https://fonts.googleapis.com/css?family=Raleway&display=swap" rel="stylesheet">
</head>
```

## Add a favicon and other cool meta tags

```
<link rel="icon" type="image/png" href="images/favicon.png">
<meta charset="utf-8">
<title>Github pages</title>
<meta name="description" content="">
<meta name="author" content="">
```

## Basic mobile responsiveness

In CSS, the media query standard allows us to apply specific CSS rules at different screen sizes. Try to load up your website on your phone, and think about how you can use media queries to improve the usability. 

```
 /* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {...}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {...}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {...}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {...} 
```

[source](https://www.w3schools.com/css/css_rwd_mediaqueries.asp)
