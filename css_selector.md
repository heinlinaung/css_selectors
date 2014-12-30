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

8. X > Y - direct children selector
```css
div#container > ul {
  border: 1px solid black;
}
```

9. X ~ Y - sibling combinator
```css
ul ~ p {
   color: red;
}
```

10. X[title] - attribute(s) selector
```css
a[title] {
   color: green;
}s
```

11. X[href="foo"]
```css
a[href="http://net.tutsplus.com"] {
  color: #1f6053; /* nettuts green */
}
```

12. X[href*="nettus"]
```css
a[href*="tus"] {
	color:#fff; /*make it white*/
}
```

13. X[href^="http"]
```css
a[href^="http"] {
   background: url(path/to/external/icon.png) no-repeat;
   padding-left: 10px;
}
```

14. X[href$=".jpg"]
```css
a[href$=".jpg"] {
	color:red;
}
```

15. X[data-*="foo"]
```css
a[data-filetype="image"] {
	color:pink;
}
```
Tips - 
```css
a[href$=".jpg"],
a[href$=".jpeg"],
a[href$=".png"],
a[href$=".gif"] {
   color: red;
}
```
```html
<a href="path/to/image.jpg" data-filetype="image"> Image Link </a>
```
```css
a[data-filetype="image"] {
	color:pink;
}
```

16. X[foo~="bar"]
```css
a[data-info~="image"] {
	border:1px solid red;
}
```

17. X:checked
```css
input[type=radio]:checked{
	border:1px solid red;
}
```

18. X:after
```css
.clearfix:after {
    content: "";
    display: block;
    clear: both;
    visibility: hidden;
    font-size: 0;
    height: 0;
    }
.clearfix { 
   *display: inline-block; 
   _height: 1%;
}
```

19. X:hover
```css
a:hover{
	backgrond:#e3e3e3;
}
```

20. X:not(selector)
```css
div:not(#container){
	color:blue;
}
*:not(p) {
	color:green;
}
```

21. X::pseduoElement
```css
p::first-line{
	font-weight:bold;
}
```

22. X:nth-child(n)
```css
li:nth-child(3){
	color:red; /*li:nth-child(4n) target every fourth list item*/
}
```

23. X:nth-last-child(n)
```css
li:nth-last-child(2){
	color:red;
}
```

24. X:nth-of-type(n)
```css
ul:nth-of-type(2){
	border:1px solid black;
}
```

25. X:nth-last-of-type(n)
```css
ul:nth-last-of-type(2){
	border:1px solid red;
}
```

26. X:first-child
```css
ul li:first-child{
	border-top:none;
}
```

27. X:last-child
```css
ul>li:last-child{
	border-bottom:none;
}
```

28. X:only-child
```css
div p:only-child{
	color:green;
}
```

29. X:only-of-type
```css
li:only-of-type{
	font-weight:bold;
}
```

30. X:first-of-type
```css
ul:first-of-type{
	color:red;
}
```