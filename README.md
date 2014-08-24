  PHP Hooks API, A plugin system solution with PHP
==========================================================

Version: 1.2 <br/>
License: http://www.gnu.org/copyleft/lesser.html LGPL

#0. What's this?

PHP Hooks API is a solution to attach plug-in scripts into the specified `hook` that is embedded in main codes. This API can be used to setup and embed `third party's plugins` in main code streaming, just like how it is done by [Wordpress Plugin API](http://codex.wordpress.org/Plugin_API).

![](https://github.com/ericwanghp/PHPHooks/blob/develop/phphooks.png)

#1. Terminology

**Plugin System:** help to add 3rd party's functions into program and also decoulp their codes from the main codes by storing these `plugins` in separate location(folder). It can flexibly dis/assemble these functions by adding/delecting  plugin files or folders without other affects. 

**Plugin:** one or set of functions, is stored in separate locations - `plugins folder`. It can be seamlessly integrated to the main program through attaching `hooks`. 

**Hook:** Plugin system use the hook method to allow the `plugin` to be `hooked into` main program.

**Apply Hook:** tell the main program, where/when execute the `attched` function scripts that stored in the `plugins folder`. 


#2. How To Do

Here is a example to demostrate how to use the plugin system.

**setup.php:** create the database of plugin system by providing DB informatin properly, if you need to manage plugins by backend.

**control.php:** is a example of plugins control panel, you can manage the plugins dis/activity by backend.

**init.php:** is a initiate process to

* include phphooks class and create instance
* fetch the active plugins list from DB
* set/define hook tags
* load/define plugin folder
* re-define functions for plugins

**example.php:** The example page demostrate to attach the specific plugin that's stored in `plugins` folder by applying hook in the main program.

**plugins folder:** storing third party's plugins.

**phphooks.class.php** phphooks class,  is core class of this system. include it if you want to use this system in your program.

#3. Donate to PHPHooks
[![paypal]](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=eric%2ewzy%40gmail%2ecom&lc=US&item_name=Donate%20to%20PHPHooks&no_note=0&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHostedGuest)
[paypal]:https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif "Donate to PHPHooks"