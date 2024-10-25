# HTMLMinify-Smarty

A simple Smarty filter for minifying HTML.

## Installation

Copy `HTMLMinify.smarty.php` into your installation and included it.

Then you can register the filter with smarty:

```php
$smarty->registerFilter("output", "minify_html");
```

## URLs

The URL component is also minified. You can change the protocol and URL to
assist with minifying if your `$_SERVER` attributes don't match up to the real
URL.

```php
define("HTML_MINIFY_URL", "https://ma.rkhugh.es");
```

Or if you don't want this feature you can disable it like this:

```php
define("HTML_MINIFY_URL_ENABLED", false);
```

## Inline CSS

By default we minifying inline CSS. You can disable it like this:

```php
define("HTML_MINIFY_INLINE_CSS_ENABLED", false);
```

## Server Side Includes (SSI)

By default we remove all comments, to keep SSI comments you can define this:

```php
define("HTML_MINIFY_KEEP_SSI", true);
```
