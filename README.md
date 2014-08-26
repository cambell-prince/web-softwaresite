Wordpress Multi-Site for Software Sites
=======================================

## Installation ##

First clone this repository.

Install the php packages, this can take awhile. Note that you must have [composer](https://getcomposer.org/) installed to do this.

```
cd htdocs
composer install
```

Install the node packages. We're using [gulp](http://gulpjs.com/) as our build runner which requires node and is available as a node package.

`npm install`

If you are working on a theme for the site you can clone this into the folder htdocs/wp/wp-content/themes

```
cd htdocs/wp/wp-content/themes
git clone http://github.com/sometheme sometheme
```
## Theme Development ##

A sample theme is [available on github](https://github.com/cambell-prince/web-product-theme1).  Themes live in the htdocs/wp/wp-content/themes directory.

### Uploading ###

You can upload from you development machine to the server using the gulp upload target.

`gulp upload`

### Live Reload ###

A live reload server is available via the gulp live reload plugin. This can be used to watch the (built) theme files and cause a page refresh whenever they change.  Saves a whole heap of wear and tear on the F5 key.

