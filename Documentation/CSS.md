<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://play-lh.googleusercontent.com/RTAZb9E639F4JBcuBRTPEk9_92I-kaKgBMw4LFxTGhdCQeqWukXh74rTngbQpBVGxqo=w480-h960" alt="Project logo"></a>
</p>
<h3 align="center">An introduction to CSS</h3>
<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
</div>

---

<p align="center">Small introduction to CSS, its Syntax and usages, from a small free bootcamp from </p>

<div align="center"> 

[www.codeinstitute.net](https://www.codeinstitute.net)
</div>

## 📝 Table of Contents

- [About](#about)
- [CSS Rules](#css_rules)
- [Selectors](#selectors)
- [Apply to multiple files](#tests)

## 🧐 About <a name = "about"></a>

CSS stands for Cascading Style sheets, it is the preferred way of setting the feel and look of a website. With it you can define and modify the color, size or position, among other things, of elements in a page.
 
## 🏁 CSS Rules <a name = "css_rules"></a>

<p align=center>
<image width=50% src="./assets/css_rules1.png" >
</p>

A rule is made out of one or more selectors inside of curly brackets, here goes the declaration where you will find the property and the value, both separated by a colon and ended by a semicolon.

```css
	/* P is the selector for parragraph element */
	p{color:teal;}
```

There are 4 different ways of including CSS in HTML:

## 1. Inline Style 

Here we apply directly to individual elements the `style` attribute.
```css
<body>
	<h1 style="color:gold;" >Why is HTML so successful?</h1>
	<p style="color:darkslategray;">
	Html is <em style="font-size:20px;">easy</em> <br>Html is <strong style="font-size:24px;">fun
	</p>
</body>
```
## 2. Style  element

This element should appear as a child element of the `<head>` element on your page.

```css
<head>
	<style type ="text/CSS">
	.auto-style1{
		text-align:right;
		background-color:purple
	}
</head>
````
## 3. Link element

This links to an external set of style rules defined in a separate file

```html
<head>
	<link ref= 'stylesheet' href=examples.css" type="text/css">
</head>
```
## 4. Import Element

Works similar to the link element but must be defined in a separate file of its own.

Here is an example of CSS applied to an HTML document

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Day 2 Challenge 1</title>
	<style>
		body {
			font-size: 14px;
		}
		/* place your style rules below this comment */
		h1{color:gold;}
		p{color:darkslategray;}
		em{font-size:20px;}
		strong{font-size:24px;}
		<h1>Why is HTML so succesful?</h1>
		<p>
		    Html is <em>easy</em>
		    Html is <strong>fun</strong>
		</p>
	</style>
  </head>
  <body>
	  <!-- give these elements some style -->
	  <h1>Why is HTML so successful?</h1>
	  <p>Html is <em>easy</em></p>
	  <p>Html is <strong>fun</strong></p>
	  
  </body>
</html>
```
And here is the result of our styling:

<h1 style="color:Gold">Why is HTML so successful?</h1> 
<p style="color:darkslategray;">
Html is <em style="font-size:20px;">easy</em> <br>Html is <strong style="font-size:24px;"> fun</strong>

# Selectors <a name = "selectors"></a>

In CSS, selectors are patterns used to select the element(s) you want to style.

here are some common selectors that can be applied as attributes.


### -  ID Selector 

Attributes are additional pieces of information that describe an element and all elements of a page can be uniquely identified on a page by means of an `ID Attribute`, this lets us group stylings into ids. the syntax of the ID element can be implemented  like this: 
```css
#id {
	css declarations;
} 
```

### -  Class Selector 

The .class selector selects elements with a specific class attribute. To select elements with a specific class, write a period (.) character, followed by the name of the class.

```css
.class {
  css declarations;
} 
```


## 🔧 Creating a cascade to apply in multiple files <a name = "tests"></a>

We can target multiple elements and even multiple files with one Styling cascade, for example

```css
	body{
		font-family:Arial;
		color:Slategray;
	}
	h1{
		font-size:300% // here is good to use porcentages, sice they adapt to devices
	}
	h1,h2{  /* we can target multiple type selectors at the same time  */
		color:orange;
		text-transform:uppercase;
		font-weight:100;
	}
	img{
		width:100%;
	}
	footer{
		margin-top:30px; /* this means push the content x pixels below the previous element*/
		background-color:slantgrey;
		color:white;
	}

	footer p{ /* In order to target a child element of our footer, in this case a parragaph, we separate the type selectors with a space*/
		text-aling:right;
		margin-left:20px;
		padding-top:20px;
		padding-bottom:20px;
	}
```

___
<div>

Now, in order to create __flow__ within our page (this means compatibility across devices), lets see some implementations of a concept called <u>__*Media Queries*__</u>


- #### <u>Media Queries</u>

Media queries allow you to apply CSS styles depending on a device's general type (such as print vs. screen) or other characteristics such as screen resolution or browser viewport width. 

```css
	body{
		font-family:Arial;
		color:Slategray;
	}
/* Here we will create an ID for our elements like images and text */
	#container{
		width:60%; /* It will be 60% of whatever screen is shown on*/
		margin:auto; /* this will center our content*/
	}
	h1{
		font-size:300% // here is good to use porcentages, sice they adapt to devices
	}
	h1,h2{
		color:orange;
		text-transform:uppercase;
		font-weight:100;
	}
	img{
		width:100%;
	}
	footer{
		margin-top:30px;
		background-color:slantgrey;
		color:white;
	}
	footer p{
		text-aling:right;
		margin-left:20px;
		padding-top:20px;
		padding-bottom:20px;
	}
	/*Here is our Media Querie, and what it means is
	that on devices below the given pixelsthe styles
	that we already have will be aplied but beyond
	that the DEFAULT styles will be applied */

	@media screen and (max-width:768px){
		#container{		/*Reuse the #container style rule inside the media query */
			width:90%;
		}
		h1{
			font-size:200%
		}
	}
```