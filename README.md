# callumacrae/960 #

callumacrae/960 is a very simple implementation of the 960 grid system, seen in the Bootstrap and 960.gs frameworks, in LESS.

## Importing it into your project ##

Simple either include the compiled CSS file, or add the following line to your LESS file:

```css
@import "960.less";
```

## Usage ##

Each "row" (marked by a div with that id) is 12 columns wide. You then specify how wide you want your columns to be using data attributes:

```html
<div class="row">
	<div data-cols="8">
		This div is 8 columns wide.
	</div>
	<div data-cols="4">
		This div is 4 columns wide.
	</div>
</div>
```

`data-cols` can be any number between 1 and 12.


At the top of 960.less, there are two variables:

```less
@gridColWidth: 60px;
@gridGutterWidth: 20px;
```

`@gridColWidth` is the width of each column, and `@gridGutterWidth` is the width of the gutter - the space between columns. Adjusting these will adjust the overall width of the row.


## Dependencies ##

This project has no dependencies (not even jQuery).


## Author ##

This project was written by Callum Macrae.
