# Swipe - a lightweight jQuery plugin

This is a lightweight jQuery plugin that allows you to monitor user swipes. 

## Getting started

###Prerequisites

This plugin requires the latest version of jQuery

###Usage

Include above `</body>` tag, but below jQuery include script tags.
```html
<script src="js/swipe.js"></script>
```
Hook to the element which you wish to observe like so:
```javascript
$(element).onSwipe();
```
.onSwipe() accepts a few parameters in the following order:

```javascript
onSwipe(function(result), timeTreshold, tresholdX, tresholdY);
```

**function(result)** - Required! A function that will handle results of swiping

***timeTreshold*** - A treshold below which swipes will not register. (ms)

***tresholdX*** - A treshold below which swipes will not register on the horizontal axis. (px) 
***tresholdY*** - A treshold below which swipes will not register on the vertical axis. (px)

Results are returned in the following object:
```json
{
	up:true/false
	right:true/false,
	down:true/false,
	left:true/false,
}
```

##Author

This project was developed by [Gvozden Despotovski](https://github.com/dsheedes/ "Gvozden Despotovski").

##License

This project is licensed under the MIT License - see the LICENSE.md file for details
