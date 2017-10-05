# Class 12
### View [all class list](https://github.com/poloey/feni)

# JavaScript Selector
In javascript, selector will return us string or array. When we select single element like body, title, head, id it will give us string. When we select multiple element like html tag, class selector return us an array. 
We can change/mutate string return. Therefore in order to change array we have to change/mutate by  destructuring array into string. 
let string selector 
~~~html
<h1 id="hello">some id heading</h1>
~~~
We can change by following code
~~~js
var heading = document.getElementById('hello');
heading.innerHtml = 'Some id heading from js';
~~~
let array selector
~~~html
  <h1 class="row">some class heading</h1>
  <h1 class="row">some class heading</h1>
  <h1 class="row">some class heading</h1>
  <h1 class="row">some class heading</h1>
  <h1 class="row">some class heading</h1>
~~~
We can change by following code. 
~~~js
var heading = document.getElementsByClassName('row');
heading[0].innerHtml = 'Some class heading from js';
~~~

In state above code we destruct heading into string then changed to its value.


### To select document
~~~js
document
~~~
### To select head
~~~js
document.head
~~~
### To select title
~~~js
document.title
~~~
### To select class
~~~js
document.getElementsByClassName('class name');
~~~
### To select id
~~~js
document.getElementById('idname');
~~~
### To select html tag element
~~~js
document.getElementsByTagName('html tag');
~~~

# New javascript query selector
In new javascript, we can select dom element using css selector. Its actually cut all complexity of javaScript selection.
### to select singular value like id, single element
~~~js
var hello = document.querySelector('#hello');
hello.innerHTML = 'some html content by js';
~~~
### To select multiple/plural value
~~~js
var row = document.querySelectorAll('.row');
row[0].innerHTML = 'some html content by js';
~~~
`querySelectorAll` return an array. We can't change array directly in js. We can change only string. So we destruct array by its index and change the content or style 
### to change style
~~~js
var hello = document.querySelector('#hello');
hello.style.color = 'red';
hello.style.fontFamily = 'sans-serif';
hello.style.fontSize = '16px';
~~~
