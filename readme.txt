=== Text Menu FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, menu, text, as3, effect, xml, vertical, horizontal, button, roll, over, out
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

A versatile free Text Menu. Fully XML customizable without any Flash knowledge. And it's free!

== Description ==

The Text Menu FX can be embedded in any website for free without even using Flash. The overall width and height can be customized up to 1680 x 1050 pixels. The menu can have an unlimited number of text items. Any type of font can be embedded but only using Flash. You can have multiple menu orientations, text orientations and menu alignment. Any colors can be used for both the text and the item background, and also roll over effects can be applied. Text padding can be specified relative to the item's background, and corner radius. Custom expanding direction for the items and scale ratio. Multiple tween functions and durations can be used for both expanding and color tween effects. Specify in the XML file the URL to go to when clicking an item.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/text-menu-fx.zip "Text Menu FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/text-menu.zip "Text Menu FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **text-menu-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Text Menu FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[text-menu-fx][/text-menu-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Text Menu FX part of your theme, edit the template files and add `<?php textmenufx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Text Menu FX](http://www.flashxml.net/text-menu.html "Text Menu FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/text-menu-fx/settings.xml`

= Additional settings file =

To embed the Text Menu FX more than once, you will need another settings file. Let's assume your new file is called `settings2.xml`. Add `[text-menu-fx settings="settings2.xml"][/text-menu-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `textmenufx_echo_embed_code()` function call (for example `<?php textmenufx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[text-menu-fx]` and `[/text-menu-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `textmenufx_echo_embed_code()` function call (for example `<?php textmenufx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[text-menu-fx width="600" height="300"][/text-menu-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `textmenufx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/text-menu.html "Text Menu FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/text-menu-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/text-menu.html "Text Menu FX") is the utility that helps easily customize your Text Menu FX to fit all your needs.