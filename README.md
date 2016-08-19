plugin.image.piwigo
====================

An Kodi (XBMC) add-on that let you browse (images and videos) from a public (or protected) [Piwigo](http://piwigo.org/) gallery instance.

Installation
------------

The add-on depends on the Kodi add-on "simplejson" to communicate with Piwigo..

**Kodi add-on plugin.image.piwigo**

 - Download the add-on as a ZIP file from GitHub
 - Open Kodi
 - Go to `System -> Settings -> Add-ons -> Install from zip file`
   - Select the previously download file 
 - Go to `System -> Settings -> Add-ons -> Enabled add-ons -> Picture add-ons -> Browse Piwigo`
   - Configure the plugin
 - Go to `Picture -> Add-ons -> Browse Piwigo`
   - Enjoy

Requirements to use size option
------

1) install/activate [extension by Piwigo Team] LocalFiles Editor from screen [Administration > Plugins > Manage]

2) open [Administration > Plugins > LocalFiles Editor > Local config] and paste the following code:
Code:

````php
$conf['question_mark_in_urls'] = false;
$conf['php_extension_in_urls'] = false;
$conf['category_url_style'] = 'id-name';
$conf['picture_url_style'] = 'file';
````

3) create a .htaccess file in the root directory of your Piwigo installation or open the existing .htaccess file.
Add the following two lines to the file and save it.

````
AcceptPathInfo On
Options +MultiViews
````
   
Support
------

To get support, please create new [issue](https://github.com/abrenoch/piwigo-kodi/issues)

Help me improve the Kodi add-on, rate my [plugin](http://piwigo.org/ext/extension_view.php?eid=770), and if possible please send a greeting message to me ;)

You can follow the discussion on the [Kodi Forum](http://forum.kodi.tv/showthread.php?tid=202393) or on the [Piwigo Forum](http://piwigo.org/forum/viewtopic.php?pid=159813)

Thanks
------

* [Kodi](http://kodi.tv/)

Licence
-------
The piwigo-kodi add-on for Kodi is free software:  you can redistribute it
and/or  modify  it under  the  terms  of the  GNU  General  Public License  as
published by the Free Software Foundation.

This program  is distributed in the hope  that it will be  useful, but WITHOUT
ANY WARRANTY; without even the  implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

See <http://www.gnu.org/licenses/gpl.html>.

