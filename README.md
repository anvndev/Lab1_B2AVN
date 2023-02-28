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
```
DOM Traversal and Manipulation
Get the <button> element with the class 'continue' and change its HTML to 'Next Step...'

$( "button.continue" ).html( "Next Step..." )
Event Handling
Show the #banner-message element that is hidden with display:none in its CSS when any button in #button-container is clicked.

var hiddenBox = $( "#banner-message" );
$( "#button-container button" ).on( "click", function( event ) {
  hiddenBox.show();
});
Ajax
Call a local script on the server /api/getWeather with the query parameter zipcode=97201 and replace the element #weather-temp's html with the returned text.

$.ajax({
  url: "/api/getWeather",
  data: {
    zipcode: 97201
  },
  success: function( result ) {
    $( "#weather-temp" ).html( "<strong>" + result + "</strong> degrees" );
  }
});
