# jQuery.SelectListActions

jQuery.SelectListActions is a jQuery plugin that gives you several actions to perform with Select lists.

With this plugin you can:

 * Move selected item(s) from a source list to a destination list
 * Move all items from a source list to a destination list
 * Move selected item(s) from a source list to a destination list and deleting the selected item(s) from the source list
 * Move all items from a source list to a destination list and deleting all items from the source list
 * Remove selected item(s) from a list
 * Move selected item(s) up or down a list

## Usage

Include **jquery.selectlistactions.js** in your page

```html
<script src="js/jquery.selectlistactions.js"></script>
```

And then make your calls like this:

**Scenario 1**: You have two lists and a button to move selected items between the lists, simply add the following:

```javascript
$('#buttonId').click(function (e) {
    $('select').moveToList('#sourceListId', '#destinationListId');
    e.preventDefault();
});
```
**Scenario 2**: You want to remove one or more items from a list

```javascript
$('#buttonId').click(function (e) {
    $('select').removeSelected('#sourceListId');
    e.preventDefault();
});
```

**Scenario 3**: You want to move selected items up in a list

```javascript
$('#buttonId').click(function (e) {
    $('select').moveUpDown('#sourceListId', true, false);
    e.preventDefault();
});
```

**Scenario 4**: You want to move selected items down in a list

```javascript
$('#buttonId').click(function (e) {
    $('select').moveUpDown('#sourceListId', false, true);
    e.preventDefault();
});
```

## Demo

I have included an **Example** folder in this repository that is styled with Bootstrap and some custom CSS.

The examples included are responsive and will look good in desktop as well as mobile.

Take a look at the [JSFiddle](http://jsfiddle.net/nzdak7aL/1/) for quick view 

**enjoy!**

 -Esau Silva
