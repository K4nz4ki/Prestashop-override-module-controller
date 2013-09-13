# Prestashop override module controller (PHP)

Allow to overrride any Prestashop module controller in `themes/[YOURTHEME]/modules/[THEMODULE]/controllers/front/[THEMODULECONTROLLER].php`


## Installation

Symply download this two classes and put them into your `override/classes/` directory.
Be careful, if the Dispatcher.php file is already present in the directory, just copy / paste the dispatch() method in your file. 

## Usage

Create a controller file with the same filename of the original module controller

`themes/my_theme/modules/loyalty/controllers/front/default.php`

Declare your controller class with the original class name of the controller you want to override. And then extend the parent class just by adding a "ModuleController" suffix

```php
<?php
class LoyaltyDefaultModuleFrontController extends LoyaltyDefaultModuleFrontControllerModuleController
{

}
```

And write your override code 

```php
<?php
class LoyaltyDefaultModuleFrontController extends LoyaltyDefaultModuleFrontControllerModuleController
{
	public function initContent()
	{
		//Your code 

		parent::initContent();
	}
}
```