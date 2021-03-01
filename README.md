## Internal Links and Ids

We have our initial heading and paragraph and contents page (the scaffold contains starter code, feel free to replace with what you had before) but we can see that each one of those list items on wikipedia take us to a place inside the webpage. Lets do that.

Each one of our `<li>` elements should contain an anchor tag, this is what is going to move us to sections of our webpage.Update your `<li>` so that the text within is wrapped by an `<a>` tag. Our `<a>` tag needs a special attribute called href, for now give the href attribute a value of "#". Like this:

```html 
<li><a href="#">This is a list item which is also a link</a></li>
```


You'll see that your list items *look* like links but they don't actually go anywhere, what we need is content to go to. Create some `<h4>` elements that we want our links to navigate to. Give each one of these h4 elements a paragraph tag and fill it in with some information like you did for the previous exercise. Lastly, give each one of these h4/paragraph combinations an accompanying image. Remember that an `<img>` has a src attribute that specifies where that image is coming from, it can either be an online image or saved locally in the workspace. You'll either have to download the image yourself and place it in the directory, or reference the online version, both ways are done in the solution that you can check for yourself.

Before we move onto the links, the images we've rendered might be too small or too large or not of a uniform size. Lets resize them by adding a height and width attribute to each of the `<img>`, lets start off small with a height and width of "400" each.

Now the fun stuff, we have links that don't go anywhere and now we have a place that we want our links to go to. External anchors we an anchor <a> element and give it a href attribute with a value of wherever we want to go, for example

```html
<a href="https://www.google.com">Click Here to go to google</a>
```

will create a link like this

[Click Here to go to google](https://www.google.com)

But we don't want to go to an external site, we want our link to take us to an internal section of our site. To do this, we need to give each of our `<h4>` elements an id attribute and a value, for now lets just give each h4 an id with the value of "one" or "two" or "three" etc for each of the headings you have eg

```html
<h4 id="one">This is my first h4 on the page</h4>
<h4 id="nine">Ths is my ninth h4 on the page</h4>
```

Each one of those ids are unique, there shouldn't be any elements that have the same id value. Now that we have something unique about each h4 we have can use that unique id to tell our \<a> tags where on the page to go to. So in the first \<a> you made update the href attribute value to "#one", we want this anchor to go to the element that has the id="one". The "#" inside the href is important as it tells the \<a> that the destination is inside of the page.

---

Now that we have that working lets take it one step further, after we've clicked a link and been taken down the page we have to scroll all the way back up to get to the contents list. That's annoying for a user and a bad user experience, lets fix that. 

Underneath each `<h4>` lets put an anchor which will travel directly to the contents list.

Once you think you're done check the solution to cross check your syntax.


