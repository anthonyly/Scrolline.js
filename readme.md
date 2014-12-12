Scrolline.js
========================================

A jQuery plugin. Create a scroll line bar indicator on the page.

## Demonstration

* [Anthonyly.com/jquery.plugins/scrolline](http://anthonyly.com/jquery.plugins/scrolline)

## Documentation

### Basic Usage

Include scrolline.js file in the page, along with jQuery.

```html
<script src="js/jquery.js"></script>
<script src="js/scrolline.js"></script>
```

Then call ``$.scrolline();`` to launch the plugin.

### Options

You can apply a set of optional options:

* ``backColor`` - Define the color of back's scrolline (default ``'#ecf0f1'``)
* ``direction`` - Can be **vertical** or **horizontal** (default ``'horizontal'``)
* ``frontColor`` - Define the color of front's scrolline (default ``'#2ecc71'``)
* ``opacity`` - Define alpha's scrolline, value must be between **0** and **1** (default ``1``)
* ``position`` -  Define the position of scrolline : **top** and **bottom** for horizontal's position, **left** or **right** for vertical's position (default ``top`` in horizontal and ``left`` in vertical)
* ``reverse`` - Revert the front line sens on set value at **true** (default ``false``)
* ``weight`` - Define the larger of scrolline on pixels (default ``5``)
* ``zindex`` - Change the z-index value if needed (default ``10``)
* ``scrollEnd`` - Callback's **function** call at the end of scrolling

### Example

Scrolline revert with custom color at bottom position:

```js
$.scrolline({
    reverse : true,
    position : 'bottom',
    backColor : '#2980b9',
    frontColor : '#f1c40f',
    weight : 12
});
```

Scrolline vertical at right position with callback:

```js
$.scrolline({
    position : 'right',
    direction : 'vertical',
    weight : 30,
    scrollEnd : function() {
		alert('End of scroll!');
	}
});
```

## Compatibility

* Safari
* Firefox
* Chrome
* IE
* Safari mobile

## Credits

### Author
[Anthony Ly](http://anthonyly.com), on twitter [@Pik_at](http://twitter.com/pik_at)

### Licence
Licence MIT