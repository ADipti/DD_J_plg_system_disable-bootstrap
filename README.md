# DD_J_plg_system_disable-bootstrap
is a reliable and extendable **Joomla! system plugin for template developers to disable Bootstrap** from the front end!

-
In the front end of Joomla! some extensions calling the function JHTML::_('behavior.tooltip'), which adds Bootstrap JavaScript to html head. To avaiod this manually by hard coding, your scripts could be broken because of an assigned "jQuery hasTooltip" function.

**Here DD Disable Bootstrap helps:** This plugin unsets Bootstrap JavaScript files and also removes hasTooltip function from front end, to disable Bootstrap and also avoid errrors which can result from the Bootstrap JS removal.

This plugin use the following snippet to remove:

    jQuery('.hasTooltip').tooltip({"html": true,"container": "body"});

If you know what you're doing, you can change the following snipped at plugin settings if it differs from your version!

    {"html": true,"container": "body"}

**Note:** It is not recommended to use together with Joomla! default templates like tpl_Protostar!

# System requirements
Joomla 3.x +                                                                                <br>
PHP 5.6.13 or newer is recommended.

# DD_ Namespace
DD_ stands for  **D**idl**d**u e.K. | HR IT-Solutions (Brand recognition)                   <br>
It is a namespace prefix, provided to avoid element name conflicts.

<br>
Author: Didldu e.K. Florian Häusler https://www.hr-it-solution.com                          <br>
Copyright: (C) 2011 - 2016 Didldu e.K. | HR IT-Solutions                                    <br>
http://www.gnu.org/licenses/gpl-2.0.html GNU/GPLv2 only
