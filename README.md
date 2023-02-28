# Lab1_B2AVN
<p align="center">
	<img src="https://raw.githubusercontent.com/anvndev/Lab1_B2AVN/master/Lab1_B2AVN/images/demo.jpg">
</p>


```html
<!--Javascript-->
<script type="text/javascript">
    function buyNow() {
        question = confirm("Do you want to buy this product?");
        if (question != false) {
            alert('Thank you for buying!!!')
        }
    }

</script>
```
----------
```
$npm i bootstrap@5.3.0-alpha1
```
-------------
# https://jquery.com/
## DOM Traversal and Manipulation
<h2>Get the <button> element with the class 'continue' and change its HTML to 'Next Step...'</h2>
	
```	
$( "button.continue" ).html( "Next Step..." )
```	
## Event Handling
<h2>Show the #banner-message element that is hidden with display:none in its CSS when any button in #button-container is clicked.</h2>
	
---------------
```
var hiddenBox = $( "#banner-message" );
$( "#button-container button" ).on( "click", function( event ) {
  hiddenBox.show();
});
```


## Ajax
<h2>Call a local script on the server /api/getWeather with the query parameter zipcode=97201 and replace the element #weather-temp's html with the returned text.</h2>

```	
	
$.ajax({
  url: "/api/getWeather",
  data: {
    zipcode: 97201
  },
  success: function( result ) {
    $( "#weather-temp" ).html( "<strong>" + result + "</strong> degrees" );
  }
});
```
	by anvndev
```
<p href="https://anvndev.github.io/Lab1_B2AVN/Lab1_B2AVN/index.html">Link Demo</p>

