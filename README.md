#Flip Out Cards by Pete R.
Create a Dynamic Multi Level Flip Out Cards
Created by [Pete R.](http://www.thepetedesign.com), Founder of [Travelistly](http://www.Travelistly.com) and [BucketListly](http://www.bucketlistly.com)

[![Flip Out Cards](http://www.thepetedesign.com/images/flipout_cards_image.png "Flip Out Cards")](http://www.thepetedesign.com/demos/flipout_cards_demo.html)

## Demo
[View demo](http://www.thepetedesign.com/demos/flipout_cards_demo.html)

## Compatibility
Modern browsers such as Chrome, Firefox, and Safari on both desktop and smartphones have been tested. I have not tested this on IE.

## Basic Usage
To create a flip out cards that shows more info when hover, simply include the latest jQuery library together with `jquery.flipout_cards.js` and `flipout_cards.css` into your document's `<head>`, and call the function as follows:

````javascript
  $(".flipout").flipout_cards({
    animation: "flipOut",           // Animations available are: flipOut, slideOut and foldOut. The default value is flipOut
    beforeOpen: function () {},     // This option accepts a callback function. The function will be called before the flip open animation starts.
    afterOpen: function () {},      // This option accepts a callback function. The function will be called after the flip open animation finishes.
    beforeClose: function () {},    // This option accepts a callback function. The function will be called before the flip close animation starts.
    afterClose: function () {}      // This option accepts a callback function. The function will be called after the flip close animation finishes.
  });
````

Now all you have to do is follow this HTML markup as shown below:

````html
<div class="flipout">
  <div class="foc-main">
    ...
  </div>
  <div class="foc-left">
   ...
  </div>
  ...
</div>
````
The container with the class name `foc-main` will be the main content area where the cards will flip out from. All the other containers below that will be the cards itself. You can have as many cards as you like. Simply duplicate the container with the class name `foc-left` and the plugin will automatically stack it all up in order.

You can also define which direction the cards will appear by simply changing the class name of the cards' container. Available class names are `foc-left`, `foc-right`, `foc-top`, and `foc-bottom`.

## Callbacks
You can use callbacks to perform actions before or after the card displays:

### beforeOpen
This option accepts a callback function. The function will be called before the flip open animation starts.

````javascript
$(".flipout").flipout_cards({
  beforeOpen: function () {
    ...
  }
});
````

### afterOpen
This option accepts a callback function. The function will be called before the flip open animation finishes.

````javascript
$(".flipout").flipout_cards({
  afterOpen: function () {
    ...
  }
});
````

### beforeClose
This option accepts a callback function. The function will be called before the flip close animation starts.

````javascript
$(".flipout").flipout_cards({
  beforeClose: function () {
    ...
  }
});
````

### afterClose
This option accepts a callback function. The function will be called before the flip close animation finishes.

````javascript
$(".flipout").flipout_cards({
  afterClose: function () {
    ...
  }
});
````

And that's all for the flip out cards plugin. I hope you will find this useful. Stay tuned for more updates.

If you want to see more of my plugins, visit [The Pete Design](http://www.thepetedesign.com/#design), or follow me on [Twitter](http://www.twitter.com/peachananr) and [Github](http://www.github.com/peachananr).

## Other Resources
- Tutorial (Coming Soon)
