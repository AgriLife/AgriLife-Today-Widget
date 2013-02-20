# Texas A&M AgriLife Today Widget
Creates a widget to display stories from today.agrilife.org.

### Note
This code originally lived in the AgriFlex theme. We took it out for portability. And because we're awesome.

## Overriding these styles in your own theme
To create your own CSS for this widget, just add the following code to your `functions.php`:

`remove_action( 'wp_enqueue_scripts', 'agrilife_today_load_styles' );`

## Changing the date format
By default this widget has a date format of `M d`. You can change it using any valid [PHP date format][1]
`add_filter( 'agrilife_today_date_format', 'm d Y' );`

[1]:http://php.net/manual/en/datetime.formats.date.php
