# jQuery SimplePagination

SimplePagination is a small jQuery plugin that can paginate a large HTML table. You can specify the number of rows to show per page and the styling for the 
pagination features.

## Setup

Include the plugin _after_ the jQuery library:
```html
<script src="/path/to/jquery.js"></script>
<script src="/path/to/jquery.simplePagination.js"></script>
```

## Usage

Create your HTML table.
```html
<table id="pages">
	<tr>
		<td>1.</td>
		<td>William Hartnell</td>
	</tr>
	<tr>
		<td>2.</td>
		<td>Patrick Troughton</td>
	</tr>
	..
	<tr>
		<td>12.</td>
		<td>Peter Capaldi</td>
	</tr>
</table>
```

Give the table some pages:
```javascript
$("#pages").simplePagination();
```

This will add pagination buttons below your table along with text for the row count and current page. 

Let's show ten (10) records per page, start on the second page, and add Bootstrap styling to the pagination buttons:
```javascript
$("#pages").undoCountdown({
  perPage: 10,
  currentPage: 2
});
```

## Options

| Name  | Type | Description | Values | Default | 
|:----- |:---- |:----------- |:------ |:------- |
| perPage | Number | The number of rows per page | Number | 5 |
| containerClass | String | Class name(s) for the pagination containing div | String | "" |
| previousButtonClass | String | Class name(s) for the previous button | String | "" |
| nextButtonClass | String | Class name(s) for the next button | String | "" |
| previousButtonText | String | The text to show on the previous button | String | "&larr; Previous" |
| nextButtonText | String | The text to show on the next button | String | "Next &rarr;" |
| currentPage | Number | The page to begin on | Number | 1 |

## Demo

Working samples can be seen [here](http://smarulanda.github.io/jquery.simplePagination/).