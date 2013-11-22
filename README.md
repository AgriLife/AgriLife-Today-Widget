# Texas A&M AgriLife Today Widget
__Description:__ Creates a widget to display stories from today.agrilife.org.
__Author:__ Texas A&M AgriLife Communications
__Version:__ 1.1

### Note
This code originally lived in the AgriFlex theme. We took it out for portability. And because we're awesome.

## Overriding these styles in your own theme
To create your own CSS for this widget, just add the following code to your `functions.php`:

`remove_action( 'wp_enqueue_scripts', 'agrilife_today_load_styles' );`

## Changing the date format
By default this widget has a date format of `M d`. You can change it using any valid [PHP date format][1]
`add_filter( 'agrilife_today_date_format', 'm d Y' );`

## Changelog

### 1.1

- Now pulls default image from plugin and not the theme

### 1.0

- Removed this functionality from AgriFlex

[1]:http://php.net/manual/en/datetime.formats.date.php
