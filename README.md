# Red Green Blue

## Exercise with Media Queries

Create a standard html5 setup linking an external stylesheet.

````
index.html
stylesheets/
  styles.css
````

Start an `http-server` in your project root.

### Set up your html5 document

1. Create an empty, basic html5 template including a doctype declaration, head, title, and body tags.
2. Set the title to `Media Queries`
1. Create a div element with an id of `container`
2. Create a div element inside of the `container` div, with an id of `hero`
3. Create a level 1 heading elemnt inside of the `hero` div, with the content of `Hello Heroes`
4. Create an unordered list element inside of the `container` div, after the `hero` div, with an id of `super_heroes`
5. Create 3 list item elements inside of the `super_heroes` unordered list element, each with content containing the name of a super hero of your choosing

````
<div id="container">
  <div id="hero">
    <h1>Hello Heroes</h1>
  </div>
  <ul id="super_heroes">
    <li>FinnMan</li>
    <li>JakeMan</li>
    <li>BMOMan</li>
  </ul>
</div>
````

### Set up your styles.css stylesheet
- Add a `link` element inside of the head tags. Set the HREF to point to your style.css file

### Set up your `index.html` page to be responsive
- Add a `meta` element inside of your `head` element. Set a `name` attribute with a value of `"viewport"`, set a `content` attribute with the value of `"width=device-eidth, initial-scale=1"`

------------------

#### Stylesheet Guidelines:

The first set of styles should apply to the page at any size.

Below the global styles, add appropriate media queries and styles for small, medium and large formats.

#### Media Query Break Points:

*Small*: max-width 40em  
*Medium*: min-width 40.063em, max-width 60em  
*Large*: min-width 60.063em  

------------------

##### General Styles:
- Your content should have a max width of 500px.
- All text should:
  - use a custom sans-serif font
  - have a base font color of dark grey

##### Small Size Only:
- The background should have a custom, medium dark red color
- The `container` div should no special formatting
- The `hero` div should:
  - be 300px tall
  - be wide enough to fill the page so that there is only 15px between the edge of this div and either edge of the page
  - have an off-white colored background
  - have a light red border with a weight of 2px
- The `super_heroes` unordered list should no special formatting
- Each list item in `super_heroes` should:
  - be 40px tall
  - be wide enough to fill the page so that there is only 15px between the edge of this div and the left and right edges of the page
  - be 15px away from other list items.
  - have an tan colored background
  - have a dark red border with a weight of 2px
  - contain text that is 15px away from this list item's borders

##### Medium Size Only:
- The background should have a custom, medium pastel green color
- The `container` div should not have any visible styles
- The `hero` div should:
  - be 200px tall
  - be the width of it's containing div
  - have an almost white background (slightly blue)
  - have a light pastel blue border with a weight of 3px
- The `super_heroes` unordered list should:
  - be tall enough to contain all of its child elements
  - be the width of it's containing div
  - be 20px away from the `hero` div
  - have an almost white background (slightly blue)
  - have a light pastel blue border with a weight of 3px
- Each list item in `super_heroes` should
  - be 300px tall
  - be 20px away from other list items.
  
##### Large Size Only:
- The background should have a custom, light pastel blue color
- The `container` div should:
  - have a light blue-greenish background color
  - have a medium blue-greenish border with a weight of 3px
- The `hero` div should:
  - be 300px tall
  - be the width of it's containing div, minus 40px
  - be 20px away from the `container` div's borders
  - have an almost white background (slightly green)
  - have no border
- The `super_heroes` unordered list should:
  - be tall enough to contain all of its child elements
  - be the width of it's containing div, minus 40px
  - be 20px away from the `hero` div
  - be 20px away from the `container` div's borders
  - have an almost white background (slightly green)
  - have no border
- Each list item in `super_heroes` should:
  - have a height of 300px tall
  - have a light gray bottom border with a weight of 1px
  
##### Large and Medium Sizes:
- each list item in `super_heroes` contains a different background image
