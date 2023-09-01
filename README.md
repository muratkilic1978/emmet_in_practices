# Learning Emmet - a powerful toolkit

Emmet is a free add-on for your text editor that allows you to type shortcuts to HTML and CSS and that increases the speed of web development. <br />Here is first a briefly documentation of how Emmet shortcuts works with HTML. Below the documentation part you will find the exercises related to Emmet. Try to solve them on your own computer. Remember hat you need to create an **index.html** to test Emmet shortcuts.

## Emmet Documentation

### The Exclamation Point

Open a new HTML file, type in !, and hit ‘Enter.’ Boom, a perfectly laid out HTML file just like that.

```emmet
!
```

Expands to

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

### Child: >

```emmet
nav>ul>li
```

Expands to

```html
<nav>
  <ul>
    <li></li>
  </ul>
</nav>
```

### Sibling: +

```emmet
section>p+p+p
```

Expands to

```html
<nav>
  <ul>
    <li></li>
  </ul>
</nav>
```

### Climb Up: ^

```emmet
section>header>h1^footer
```

Expands to

```html
<section>
  <header>
    <h1></h1>
  </header>
  <footer></footer>
</section>
```

### Grouping: ()

```emmet
section>(header>nav>ul>li)+footer>p
```

Expands to

```html
<section>
  <header>
    <nav>
      <ul>
        <li></li>
      </ul>
    </nav>
  </header>
  <footer>
    <p></p>
  </footer>
</section>
```

### Multiplication: \*

```emmet
ul>li*3
```

Expands to

```html
<ul>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

### IDs and Classes:

```emmet
ul.menu>li.menu__item+li#id_item+li.menu__item#id_2
```

Expands to

```html
<ul class="menu">
  <li class="menu__item"></li>
  <li id="id_item"></li>
  <li class="menu__item" id="id_2"></li>
</ul>
```

### Numbering: $

```emmet
ul>li.item$*3
ul>li.item$$*3
ul>li.item$@-*3
```

Expands to

```html
<ul>
  <li class="item1"></li>
  <li class="item2"></li>
  <li class="item3"></li>
</ul>
<ul>
  <li class="item01"></li>
  <li class="item02"></li>
  <li class="item03"></li>
</ul>
<ul>
  <li class="item3"></li>
  <li class="item2"></li>
  <li class="item1"></li>
</ul>
<ul>
  <li class="item3"></li>
  <li class="item4"></li>
  <li class="item5"></li>
</ul>
```

### Text: {}

```emmet
p>lorem10
```

Expands to

```html
<p>
  Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, expedita.
</p>
```

## Exercise

Download/clone this repo to your machine (Mac / Win).
Next open the **index.html** file from the repository that you downloaded above with your editor Visual Studio Code. Now try to test the different Emmet shortcuts inside the index.html file.
