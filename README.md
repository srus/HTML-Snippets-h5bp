# Sublime Text 2 HTML Snippets

_A work in progress._

Type the snippet shortcode and then press <kbd>Tab</kbd> to complete the snippet.

The snippets are listed below in alphabetical order. The '$1' indicates the
position of the caret/s. Some snippets have been set up so that pressing Tab
jumps the caret/s to the next predefined spot. It's a little hard to explain,
but any snippet that has a $1/$2/$3/etc. uses this technique.

Feel free to play with, alter, expand, or ruin these snippets as you please. I
only ask that if you come up with an incredibly handy snippet, or simply one
that I have missed, that you let me know (via email, Twitter or GitHub) so that
I can improve these for everybody. Thanks!

__IMPORTANT: If you are also using Emmet, add the following to Emmet's user settings file:__

`"disabled_single_snippets": "fig html head img link meta nav ol picture script style ul video"`

---

__a__

```html
<a href="$1">$2</a>
```

__comm__

```html
<!-- $1 -->
```

__cond__

```html
<!--[if ${1:lt IE 9}]>
    <link rel="stylesheet" href="${2:css/ie.css">}
<![endif]-->
```

__doctype__

```html
<!DOCTYPE html>
```

__fig__

```html
<figure>
    <img src="$1" alt="$2">
    <figcaption>$3</figcaption>
</figure>
```

__ga__

```html
<script>
    (function(b,o,i,l,e,r){b.GoogleAnalyticsObject=l;b[l]||(b[l]=
    function(){(b[l].q=b[l].q||[]).push(arguments)});b[l].l=+new Date;
    e=o.createElement(i);r=o.getElementsByTagName(i)[0];
    e.src='//www.google-analytics.com/analytics.js';
    r.parentNode.insertBefore(e,r)}(window,document,'script','ga'));
    ga('create','${1:UA-XXXX-X}');ga('send','pageview');
</script>
```

__head__

```html
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>${2:Untitled}</title>
    <meta name="description" content="$3">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link rel="stylesheet" href="${4:css/main.css}">
</head>
```

__html__

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <title>${1:Untitled}</title>
        <meta name="description" content="$2">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <link rel="stylesheet" href="${3:css/main.css}">
    </head>
    <body>
        $5
        <script src="${4:js/main.js}"></script>
    </body>
</html>
```

__img__

```html
<img src="$1" alt="$2" sizes="$3" srcset="$4">
```

__jquery__

```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/${1:1.10.2}/jquery.min.js"></script>
<script>window.jQuery || document.write('<script src="js/vendor/jquery-${1:1.10.2}.min.js"><\/script>')</script>
```

__link__

```html
<link rel="${1:stylesheet}" href="$2">
```

__lorem__

```html
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
culpa qui officia deserunt mollit anim id est laborum.
```

__nav__

```html
<nav class="$1">
    <ul>
        <li><a href="#">$2</a></li>
        <li><a href="#">$3</a></li>
        <li><a href="#">$4</a></li>
        <li><a href="#">$5</a></li>
    </ul>
</nav>
```

__ol__

```html
<ol>
    <li>$1</li>
    <li>$2</li>
    <li>$3</li>
    <li>$4</li>
</ol>
```

__picture__

```html
<picture>
    <source media="(min-width: ${1:800px})" srcset="${2:image.jpg}, ${3:image-2x.jpg 2x}">
    <source media="(min-width: ${4:450px})" srcset="${5:image-small.jpg}, ${6:image-small-2x.jpg 2x}">
    <img src="${7:image.jpg}" alt="$8" srcset="${9:image-2x.jpg 2x}">
</picture>
```

__script__

```html
<script src="$1"></script>
```

__style__

```html
<style>
    $1
</style>
```

__ul__

```html
<ul>
    <li>$1</li>
    <li>$2</li>
    <li>$3</li>
    <li>$4</li>
</ul>
```

__video1__

```html
<video src="${1:movie}.${2:webm}" type="video/$2" ${3:controls} poster="${4:poster.jpg}">
    <p>${5:Your browser does not support the video element.}</p>
</video>
```

__video2__

```html
<video ${1:controls} poster="${2:poster.jpg}">
    <source src="${3:movie}.${4:webm}" type"video/$4">
    <source src="${5:movie}.${6:mp4}" type"video/$6">
    <p>${7:This browser does not support the video element.}</p>
</video>
```
