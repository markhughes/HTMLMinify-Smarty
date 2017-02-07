# HTMLMinify-Smarty
A simple Smarty filter for minifying HTML.

## Installation
Copy `HMTLMinify.smarty.php` into your installation and included it.

Then you can register the filter with smarty:

```php
$smarty->registerFilter("output", "minify_html");
```
