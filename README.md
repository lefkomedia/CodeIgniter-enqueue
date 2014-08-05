CodeIgniter-enqueue
===================
Adds enqueue capabilites to CodeIgniter with a simple library.

## How to use
### Setup
1. Add `enqueue.php` to `YOUR/APP/PATH/application/libraries/`
2. Add `enqueue` to the array on Line 55: `$autoload['libraries'] = array();` in `YOUR/APP/PATH/config/autoload.php`
3. In your theme file(s) add `$this->enqueue->loadjs();` and `$this->enqueue->loadcss();` where you would like to load enqueued scripts.

### Usage
Add JS and CSS files to `YOUR/APP/PATH/public/js/` and `YOUR/APP/PATH/public/css/`, respectively. If these folders don't exist you will need to create them.

In your controllers or models add:
* `$this->enqueue->enqueue_js('JS_FILENAME');` to enqueue JavaScript
* `$this->enqueue->enqueue_CSS('CSS_FILENAME');` to enqueue CSS
