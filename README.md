# heart.js

A beating heart on canvas with audio.

The HTML:
```html
<div id="heart"></div>
```

The JavaScript:
```javascript
var myHeart = new Heart({
	target: '#heart',
	audioEnabled: true
});
```

The options with defaults:
```javascript
this.options = {
	target: null, // Selector of element or the element itself
	width: 500, // Width in pixels
	height: 500, // Height in pixels
	size: 200,
	bloat: 0.25,
	color: '#DA755C',
	audioEnabled: false,
	audio: 'audio/heart.wav',
	context: null // Specify an Audio context
};
```
