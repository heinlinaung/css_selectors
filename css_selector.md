CSS Selectors:
----------------
 - Ref : [Nettus+](http://code.tutsplus.com/tutorials/the-30-css-selectors-you-must-memorize--net-16048)


1.  \* - select all
```css
* {
 margin: 0;
 padding: 0;
}
```
```css
#container * {
 border: 1px solid black;
}
```

2. \#X - id selector
```css
#container {
   width: 960px;
   margin: auto;
}
```

3. .X - class selector
```css
.error {
  color: red;
}
```

4. X Y - descendant selector
```css
li a {
  text-decoration: none;
}
```

5. X - all specific elements
```css
a { color: red; }
ul { margin-left: 0; }
```

6. X:visited and X:link - pseudo class
```css
a:link { color: red; } /*all anchor tags which have yet to be clicked on*/
a:visted { color: purple; } /*all anchor tags which have visited/clicked on*/
```

7. X + Y - an adjacent selector
```css
ul + p {
   color: red;
}
```