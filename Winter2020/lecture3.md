# Personal site workshop 3

## Making a responsive grid layout for your website

Thanks to the magic of HTML5 + CSS3, we can define a responsive grid that reduces down to one column on mobile without writing any special rules for screen sizes. This can be useful if you're trying to make cards that display information and dynamically resize.

HTML:
```
<div class="coolGrid">
  <!-- Grid items here -->
</div>
```

CSS:
```
.coolGrid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}
```

## What's happening here?

The first line of our css defines that we're gonna be using CSS grid. The next line utilizes two CSS functions in order to define a responsive grid in one line. the minmax function lets us define the minimum and a maximum column size that we want in our grid. In this case the column can grow to 1fr on larger devices and shrink down to 300px on smaller ones. The auto-fit keyword combined with repeat() allows us to tell the browser to only have one column on smaller sizes, perfect for mobile.
