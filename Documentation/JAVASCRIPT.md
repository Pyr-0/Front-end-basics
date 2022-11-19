<p align="center">
  <a href="" rel="noopener">
 <img width=300px  src="https://1000logos.net/wp-content/uploads/2020/09/JavaScript-Logo-1024x640.png" alt="Project logo"></a>
</p>
<h3 align="center">An introduction to Javascript</h3>
<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)
</div>

---

<p align="center">Small and simple introduction to Javascript, its Syntax and usages, from a small free bootcamp from </p>

<div align="center"> 

[www.codeinstitute.net](https://www.codeinstitute.net)
</div>

## 📝 Table of Contents

- [About](#about)
- [Javascript Elements](#javascript)
- [Selectors](#selectors)

## 🧐 About <a name = "about"></a>

JavaScript is a programming language that lets you enhance your HTML with `animation`, `interactivity` and dynamic `visual effects`. It can make web pages more useful by supplying immediate feedback. \
For example, a JavaScript powered shopping cart can instantly display a total cost, with taxes and shipping, the moment a visitor selects a product to buy. 
<div align=center>
<img width=100% src="https://res.cloudinary.com/practicaldev/image/fetch/s--H7ifINUG--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zpsckl53ynytogr8qvw6.png">
</div>
JavaScript is used when determining whether the credit card details you entered are valid before transferring those details across the net to the bank for processing. JavaScript is now the language of the web.<br>
<u>HTML and CSS are concerned with how something is displayed, but JavaScript can make logical decisions.</u> <br><br>

<div align="center">
<img src="https://flatironschool.com/legacy-assets/images.ctfassets.net/hkpf2qd2vxgx/44oj2847JshvH8bktR7JyM/070c9adb7b012836066efe8ee53ae4a9/HTML_CSS_JS.gif">
</div>

## 🧐 Javascript Elements <a name = "html5elements"></a>

<div>

A web browser is usually expecting HTML where we specifically tell the browser
when JavaScript is included. To do this, we use the `<script>` tag. This is similar to the `<style>` tag used in CSS. And also like CSS, JavaScript can be included in the `<head>` element or accessed from an external file.\
For example:

```html
	<head>
		<script>
			document.getElementByld("demo")
			innerHTML= "Hello Javascript";
		</script>
	</head>
```
JavaScript doesn't have to be confined to the `<head>` element though. You can insert script elements in the body area too - creating islands of behavior, or functionality, throughout the page.
</div>

###  <u>Event handling (overview)</u>
Events are signals fired inside the browser window that notify of changes in the browser or operating system environment. Programmers can create event handler code that will run when an event fires, allowing web pages to respond appropriately to change.

In order to create handlers for events, we can create `Event Listeners`.

here is an example of a button being clicked that displays the time: 

```html
	<!DOCTYPE html>
	<html>
		<body>

			<h2>JavaScript addEventListener()</h2>

				<p>This example uses the addEventListener() method to attach a click event to a button.</p>

					<button id="myBtn">Try it</button>

				<p id="demo"></p>

			<script>
				document.getElementById("myBtn").addEventListener("click", displayDate);
				function displayDate() {
	  				document.getElementById("demo").innerHTML = Date();
				}
			</script>

		</body>
	</html> 
```

... you can then add events of different types to the same element:

```javascript
	element.addEventListener("mouseover", myFunction);
	element.addEventListener("click", mySecondFunction);
	element.addEventListener("mouseout", myThirdFunction); 
```
and with this here we create a "feedback button" for each event

```html
<!DOCTYPE html>
	<html>
		<body>

			<h2>JavaScript addEventListener()</h2>

			<p>This example uses the addEventListener() method to add many events on the same button.</p>

			<button id="myBtn">Try it</button>

			<p id="demo"></p>

			<script>
				var x = document.getElementById("myBtn");
				x.addEventListener("mouseover", myFunction);
				x.addEventListener("click", mySecondFunction);
				x.addEventListener("mouseout", myThirdFunction);

				function myFunction() {
				  document.getElementById("demo").innerHTML += "Moused over!<br>";
				}

				function mySecondFunction() {
				  document.getElementById("demo").innerHTML += "Clicked!<br>";
				}

				function ingredientsHover() {
				  document.getElementById('ingredients').firstElementChild.FirstElementChild.style.fontSize="300%";
				}
				function ingredientsNormal() {
				  document.getElementById('ingredients').firstElementChild.FirstElementChild.style.fontSize="100%";
				}
				function preparationsHover() {
					document.getElementById('ingredients').firstElementChild.FirstElementChild.style.fontSize="300%";
				}
					function preparationsNormal() {
					  document.getElementById('ingredients').firstElementChild.FirstElementChild.style.fontSize="100%";
					}
				function myThirdFunction() {
				  document.getElementById("demo").innerHTML += "Moused out!<br>";
				}
			</script>

</body>
</html>
```

