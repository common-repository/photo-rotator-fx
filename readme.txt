=== Photo Rotator FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, photo, rotator, image, text, as3, slideshow, auto, xml, effects, animation
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

Probably the most advanced Photo Rotator on the web. Completely XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. It's completely customizable and it uses HTML/CSS formatted text. It has autoplay functionality, effects like shadow and blur, background and shade features and a lot of different properties on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/photo-rotator-fx.zip "Photo Rotator FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/photo-rotator.zip "Photo Rotator FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **photo-rotator-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **Photo Rotator FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[photo-rotator-fx][/photo-rotator-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Photo Rotator FX part of your theme, edit the template files and add `<?php photorotatorfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Photo Rotator FX](http://www.flashxml.net/photo-rotator.html "Photo Rotator FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/photo-rotator-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/photo-rotator-fx/images/` and update the `wp-content/flashxml/photo-rotator-fx/images.xml` file accordingly

= Additional settings file =

To embed the Photo Rotator FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[photo-rotator-fx settings="settings2.xml"][/photo-rotator-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `photorotatorfx_echo_embed_code()` function call (for example `<?php photorotatorfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[photo-rotator-fx]` and `[/photo-rotator-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `photorotatorfx_echo_embed_code()` function call (for example `<?php photorotatorfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[photo-rotator-fx width="600" height="300"][/photo-rotator-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `photorotatorfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/photo-rotator.html "Photo Rotator FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/photo-rotator-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/photo-rotator.html "Photo Rotator FX") is the utility that helps easily customize your Photo Rotator FX to fit all your needs.