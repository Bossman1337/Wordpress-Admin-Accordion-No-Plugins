# Project Title

Wordpress Admin Accordion without 3rd party plugins. Can be used within your own plugin. Good for settings pages.

## Getting Started

For an example Wordpress accordion that is currently being used by Wordpress, you can view the site health area:

```
Tools > Site Health
```
Screenshot of Wordpress Site Health.
![WP Site Health Example](/screenshots/accordion-sample-wp-health.png?raw=true "WP Site Health Example")

## STEP 1

Add the HTML to your plugins admin settings area, wherever you need it. Example HTML found in the **example-html.php**

Change to whatever text you like. For the accordion to work make sure to change the button and corrosponding DIV ID's so they are unique to each accordion dropdown. In the example HTML i've callled them **UNIQUE_NAME_1** and **UNIQUE_NAME_2**.

## STEP 2

Copy the CSS file **wp-admin-accordion.css** to your assets and then add the jQuery code from **wp-admin-accordion.js** to your JS file.

## STEP 3

You need to enqueue the CSS so it loads on your plugin settings page (or anywhere you need).

For example:
```
wp_enqueue_style('wp_accordion_css', plugins_url('assets/css/wp-admin-accordion.css', __DIR__));
```

## STEP 4

That should be it. Clear your browser cache and it should work.

### Prerequisites

* A Wordpress installation.
* An understanding of Wordpress Plugin Development (You're creating your own plugin).

## Contributing

Feel free to update or point out any mistakes or improvments :)

## Authors

* **Ross Phillipson** - *Initial work* - [Bossman](https://github.com/Bossman1337)

See also the list of [contributors](https://github.com/Bossman1337/Wordpress-Admin-Accordion-No-Plugins/contributors) who participated in this project.

## License

This project is licensed under the MIT License.