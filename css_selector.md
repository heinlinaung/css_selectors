CSS Selectors:
----------------
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
===============
2. \#X - id selector
```
#container {
   width: 960px;
   margin: auto;
}
```

3. .X - class selector
```
.error {
  color: red;
}
```

4. X Y - descendant selector
```
li a {
  text-decoration: none;
}
```

5. X - all specific elements
```
a { color: red; }
ul { margin-left: 0; }
```

6. X:visited and X:link - pseudo class
```
a:link { color: red; } /*all anchor tags which have yet to be clicked on*/
a:visted { color: purple; } /*all anchor tags which have visited/clicked on*/
```

7. X + Y - an adjacent selector
```
ul + p {
   color: red;
}
```