# calcTable

The calcTable.js is a small jQuery plugin to sum columns' numbers.

How to use it:

1. Import the latest version of jQuery library and calcTable.js into your project:
```javascript
<script src="//code.jquery.com/jquery-3.2.0.slim.min.js"></script>
<script src="calcTable.js"></script>```
```
2. Just call the function calcTable() on the html table and the plugin will do the rest:
```javascript
$(".myTable").calcTable();
```
3. The plugin allows you to skip the first row when performing the calculating:
```javascript
$(".myTable").calcTable({
"skipFirstColumn" : true
});
```
4. Change the default 'Total' text, if you need:
```javascript
$(".myTable").calcTable({
  "totalText" : "Total"
});
```
5. Add extra CSS class(es) to the 'Total' row (next release):
```javascript
$(".myTable").calcTable({
  "totalClass": "your-class"
});
```
Example:
```javascript
<script type="text/javascript">
  $(".first").sumTable({
    "skipFirstColumn" : true,
    "totalText" : "Totais"
    "totalClass" : "anotherClassName"
  });
</script>
```
