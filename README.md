# heart.js

A beating heart on canvas with audio.

## Use

The HTML:
```html
<div id="heart"></div>
```

The JavaScript:
```javascript
var myHeart = new Heart({
	target: '#heart'
});
```

## Options

The options with defaults:
```javascript
var options = {
	target: null, // Selector of element or the element itself
	heartrate: 60, // The initial pulse setting
	width: 500, // Width in pixels
	height: 500, // Height in pixels
	size: 200, // The mid-point size
	bloat: 0.25, // Magnitude of the heart animation [+/- bloat * size]
	color: '#DA755C',
	audioEnabled: true,
	audio: 'audio/heart.wav',
	context: null // [optional] Specify an Audio context
};
var myHeart = new Heart(options);
```
If no Audio Context is given, one is created automatically.

## Control

Change the pulse using:
```javascript
myHeart.pulse(heartrate);
```
