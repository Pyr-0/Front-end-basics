<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2560px-HTML5_logo_and_wordmark.svg.png" alt="Project logo"></a>
</p>
<h3 align="center">An introduction to HTML5</h3>
<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
</div>

---

<p align="center">Small and simple introduction to HTML5, its Syntax and usages, from a small free bootcamp from </p>

<div align="center"> 

[www.codeinstitute.net](https://www.codeinstitute.net)
</div>

## 📝 Table of Contents

- [About](#about)
- [HTML5 Elements](#html5elements)
- [Selectors](#selectors)

## 🧐 About <a name = "about"></a>

The latest incarnation of HTML, called HTML 5, attempts to address the absence of semantic clarity in older HTML elements. In doing so, it has introduced what are called semantic elements. These elements clearly describe their meaning to both developers and browsers. By the way, HTML doesn't do away with the older elements. It just introduces additional elements to supplement and add context to their meaning. \
Here's a list of more common elements:

## 🧐 HTML5 Elements <a name = "html5elements"></a>


- #### <u>The Header </u>
The `<header>` element provides introductory content. A `<header>` typically contains a group of introductory or navigational aids. 

```html
	<header>
		<h1>Most important heading here</h1>
	<h3>Least important heading here</h3>
	<p>Aditional content here</p>
	</header>
```
- ####  <u>The navigation bar</u>

The `<nav>` element represents a location on a page that links to other pages or to parts within a page. It's like a `<section>` with navigation links. Note though,  that not all groups of links on a page need to be in a `<nav>` element. Only sections that consist of major navigation blocks are appropriate for the `<nav>` element. 

```html
 <ul>
	 <li><a href="default.asp">Home</a></li>
  <li><a href="news.asp">News</a></li>
  <li><a href="contact.asp">Contact</a></li>
  <li><a href="about.asp">About</a></li>
</ul> 
```

- #### <u>The Articles</u>

The `<article>` element represents an independent piece of content - that is content that makes sense on its own. This could be a blog post, a magazine, or a newspaper article, a user submitted comment, an interactive widget, or any other independent item of content

```html
	<article>
		<h1> This is a Heading </h1>
	<p> This is a Paragraph about the wedding </p>
	</article>
	<p> This is a Separate Paragraph </p>
```
- #### <u>The Sections</u>

The `<section>` element is used to represent a group of related content. This is similar to the purpose of an `<article>` element, with the main difference being that the content within a `<section>` element doesn't necessarily need to make sense out of the context of that page. A website's home page could be split into sections for an introduction, news items, and contact information. Sections could define a newspaper section, summaries and links to sports, current affairs, lifestyle, politics and arts reviews.

```html
	<section>
	<h1> This is a Section </h1>
	<p> This is a Paragraph about the Section </p>
	</section>

	<section>
	<h1> This is another Section </h1>
	<p> This is a paragraph about the SecondSection </p>
	</section></ul> 
```

Now there are many other semantic elements introduced in HTML 5 and also some semantic elements that have been around for quite a while such as the table and form elements. here are some to name a few 

- `<header>`
- `<nav>`
- `<article>`
- `<section>`
- `<table>`
- `<details>`
- `<figure>`
- `<form>`
- `<aside>`
- `<mark>`
- `<main>`

### <u>This is important because semantic elements highlight intent </u>

One functional use of HTML5 is the ability to include images by link references either of your local machine storage or web links , the syntax to use for this purpose is:

```html
	<img src="here goes your path or link to the image">
```


