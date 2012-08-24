Plugs Change Log
=====================

0.1.3 Version
-----------------

* Fix jqutils.js QueryString, you can pass url to `new QueryString(url)` now.
* Refactor createpaginatin with new query_string function.
* Refactor user_admin with: APP_LAYOUTS config
* Add alignTo=fixed support to poshytip
* Update zh_CN translation
* Improve dialog2 plugin, add field_prefix option
* Fix jqmultiselect container width bug
* Add jquery 1.8.0
* Add bootstrap 2.1.0 and remove bootstrap 2.0 and 2.0.1

0.1.2 Version
-----------------

* Improve forum upload filename convert process, add `alt=` to download href, so 
   that the download filename will use alt value.
* Fix pnotify inc_show_message js bug, change `top.$(window)` to `$(top.window)`
* Upgrade pnotify to 1.2.0
* Add backbone and underscore to plugs.ui.js.jsutils, and you can use:
    
    ```
    {{use "backbone""}}
    ```
    
   to use backbone.
* Add AngularJS in 'plugs.ui.angularjs', and you can use::
    
    ```
    {{use "angularjs"}}
    ```
    
* Add font-awesome support in 'plugs.ui.bootstrap', and you can use::

    ```
    {{use "fontawesome"}}
    ```
    
* Fix fontawesome confict with bootstrap icon class
* Upgrade bootstrap to 2.0.4
* Add slickgrid and jqevent plugin
* Fix userinfo block to user_info
* Add totop plugin
* Refactor forum to static creation
* Add bootstrap pagination function, you can call like:

    ```
    pagination = functions.create_pagination(url, total, page, rows, length=None)
    return {'pagination':pagination}
    ```
    
    and in template you can:
    
    ```
    <div class="pagination">{{<< pagination}}</div>
    ```
    
* Add jquery.cookie
* Fix bootstrap prettify theme = default bug
* Remove jqjson
* Add jqhotkeys (via jquery.hotkeys.js)
* Fix forum title display