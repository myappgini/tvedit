
# Field editor in table view

Hello in this oportunity want to leave for your programs an application that will allow you, in the tables view, to quickly edit the fields.

Updating this information via ajax.

On the server side it has all the security that appgini offers with respect to the user, executing the hooks before updating and after updating, it also records the user's update.

## Install

download from github repository:

[https://github.com/myappgini/tvedit](https://github.com/myappgini/tvedit)

## Setup

First of all you have to register the js libraries for them to run.
Find and edit the `extras-header.php` file inside the hooks folder.
Add the following two command lines:
  
    <script  src = "<?php echo PREPEND_PATH;?>LTE/plugins/jquery-jeditable/jquery.jeditable.js"></script>
    <script  src = "<?php echo PREPEND_PATH;?>LTE/tvedit/tv.edit.js"></script>

To be activated within the table view you need you must write within the table tablename-tv.js (you must create a new one if it is not found) the following command lines:

    $j(function () {
        tv_editlets (AppGini.currentTableName ());
    });

just comment on the previous line so that the application is deactivated.

Soon I will try to make it work with a plugin, to avoid having to write some code.

This application is generated with appgini's own code and will be released by jquery_jeditable

which is free to use.

The same can be found here:

https://github.com/NicolasCARPi/jquery_jeditable/

## Screenshot

![https://github.com/myappgini/tvedit/blob/master/screenshots/tvedit.png](https://github.com/myappgini/tvedit/blob/master/screenshots/tvedit.png?raw=true)

The work is provided “as is”. You may not hold the author liable.

Please, if you think there is an error, do not stop commenting, as well as if you liked it.

Thanks a lot!

I hope you enjoy it
