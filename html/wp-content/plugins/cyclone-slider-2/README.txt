=== Cyclone Slider 2 ===
Contributors: kosinix
Donate link: http://www.codefleet.net/donate/
Tags: slider, slideshow, drag-and-drop, wordpress-slider, wordpress-slideshow, cycle 2, jquery, responsive, translation-ready, custom-post, cyclone-slider
Requires at least: 3.5
Tested up to: 4.0
Stable tag: 2.8.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Create and manage sliders with ease. Built for both casual users and developers.

== Description ==

Cyclone Slider 2 is an easy-to-use slider plugin with an intuitive user interface. It leverages the built-in features of WordPress. It uses custom post for the slider, custom fields to store settings, and media uploader for the images. It also uses a template system that allows developers to easily customize the look and behavior of the slider. It's a simple and flexible slider plugin.

= Features: =
* Very easy to use interface! Just drag and drop to re-order your slides.
* Responsive slider for responsive and fluid websites.
* Supports image, YouTube, Vimeo, custom HTML, and testimonial slides.
* Powered by [Cycle 2](http://jquery.malsup.com/cycle2/), the most flexible jQuery slideshow plugin.
* Every project is unique. To address this issue Cyclone Slider 2 has a template system that allow developers to easily customize the slider appearance and behavior.
* Ability to add per-slide transition effects.
* Customizable tile transition effects.
* Unlimited sliders.
* Unique settings for each slider.
* Supports random slide order.
* Shortcode for displaying sliders anywhere in your site.
* Ability to import images from NextGEN (NextGEN must be installed and active).
* Translation ready and RTL support.
* Ability to use qTranslate quick tags for slide title and descriptions (qTranslate must be installed and active).
* Allows title and alt to be specified for each slide images.
* Comes with a widget to display your slider easily in widget areas.
* Ability to fine tune the script settings. You can choose what scripts to load and where to load them.
* It's FREE!

= Demos =
* View some [screenshots](http://wordpress.org/plugins/cyclone-slider-2/screenshots/).
* Checkout the [Cyclone Slider 2 homepage](http://www.codefleet.net/cyclone-slider-2/) for a live demo.

= Credits =
* Cyclone Slider 2 was based on [Cycle 2](http://jquery.malsup.com/cycle2/) by [Mike Alsup](http://jquery.malsup.com/).
* Special thanks to Cea Bacolor for the wonderful photos.


= Translations = 
* Aubin BERTHE for the French translation.
* maxgx for the Italian translation.
* [Hassan](http://wordpress.org/support/profile/hassanhamm) for the Arabic translation.
* Javad for the Persian translation.
* [Borisa Djuraskovic](http://www.webhostinghub.com/) for the Serbo-Croatian translation.
* [Gabriel Gil](http://gabrielgil.es/) and [Digital03](http://digital03.net/) for the Spanish translation.

Do you want to translate Cyclone Slider into your language? Go to the project page at [transifex](https://www.transifex.com/projects/p/cyclone-slider-2/), create a free account, and join.

= License =
GPLv2 or later - http://www.gnu.org/licenses/gpl-2.0.html

== Installation ==

= Install via WordPress Admin =
1. Ready the zip file of the plugin
1. Go to Admin > Plugins > Add New
1. On the upper portion click the Upload link
1. Using the file upload field, upload the plugin zip file here and activate the plugin

= Install via FTP =
1. First unzip the plugin file
1. Using FTP go to your server's wp-content/plugins directory
1. Upload the unzipped plugin here
1. Once finished login into your WP Admin and go to Admin > Plugins
1. Look for Cyclone Slider 2 and activate it

= Usage =
1. Start adding sliders in 'Cyclone Slider' menu in WordPress
1. The shortcodes and php code are generated automatically by the plugin. Just copy and paste it.


== Frequently Asked Questions ==

= Why is my slider not working? =
Check for javascript errors in your page. This is the most common cause of the slider not running. See [diagnosing javascript errors](http://codex.wordpress.org/Using_Your_Browser_to_Diagnose_JavaScript_Errors). Fix the javascript errors and the slider will run.

Also check if you are using jQuery Cycle 1 script by viewing your page source. jQuery Cycle2 won't work if both are present.

= How do I pause an auto running slider when I play a YouTube or Vimeo video? =
Sorry but its not currently supported as it requires loading the YouTube API which is an extra overhead. A solution would be to disable auto transition.

= Why is there is an extra slide that I didn't add? = 
Most probably its wordpress adding paragpraphs on line breaks next to the slides therefore adding a blank `<p>` slide. You can try adding this to functions.php:
`remove_filter('the_content', 'wpautop');`

= Where do I add my own templates? =
Inside `wp-content` create a folder named "cycloneslider". Add your templates inside.

== Screenshots ==

1. All Slideshow Screen
2. Slideshow Editing Screen
3. Slideshow in Action
4. Slideshow Widget
5. Slideshow Settings

== Changelog ==

= 2.8.4 - 2014-09-04 =
* Updated spanish language files
* Added compatibility with WP 4.0

= 2.8.3 - 2014-08-20 =
* Fix. Admin menu icon for WP 3.9+.
* Fix. Language files load path.

= 2.8.2 - 2014-01-10 =
* New. Added testimonial slide type. Now you can create testimonial sliders.
* New. Added support for testimonial slides in Dark and Standard templates.
* New. Added Spanish translation by Gabriel Gil.
* New. Added Serbo-Croation translation by Borisa Djuraskovic.
* Change. Added a few responsive tweaks in admin.css for the template selection area.
* Change. Removed unused codes. 

= 2.8.1 - 2014-01-02 =
* New. Added ability to disable related videos in YouTube slide.
* New. Slide title now appends the slide caption of there is one.
* New. MP6 color schemes. Added subtle cosmetic changes to UI depending on what admin color scheme was selected.
* Change. Made hide_non_active false only if using dynamic height and YouTube/Vimeo slides. For backwards compatibility with older templates.
* Change. Removed old problematic video slide.
* Fix. Fixed Vimeo error when URL fails to load.
* Fix. Fix for very long slide titles.
* Fix. Bug fix for PHP warning in template selection when template is unchecked in settings page.

= 2.8.0 - 2013-12-29 - This is a major release =
* New. Added support for YouTube, Vimeo and Custom slide types in Text template.
* New. Added support for YouTube and Vimeo slide types in Dark template.
* New. Added "Location" column in template selection panel.
* New. Added warning when a template is located in the currently active theme directory. It warns the user of potential deletion of the template when a theme is updated.
* New. Added template directory in wp-content/cycloneslider/. This is now the recommended directory to store custom or modified templates to survive update nukes.
* New. Added width_management to shortcode attributes.
* Change. hide_non_active is now always set to false for getBoundingClientRect to not return zero.
* Fix. Minor change for directory separator on active theme location.
* Fix. Fixed inacurate next slide height reading by using getBoundingClientRect() instead of outerHeight().
* Fix. Added check to fix PHP warning when Vimeo URL is blank.

= 2.7.7 - 2013-11-26 =
* New. Added ability to select multiple images to add as slides
* Change. Refactor code for template javascripts. Moved similar code into client.js

= 2.7.6 - 2013-10-13 =
* New. Added support for YouTube and Vimeo slide types in thumbnails template.
* New. Added ability to fetch thumbnails of videos from youtube.com and vimeo.com. The thumbnails template will use this to display the thumbnails in its pager.

= 2.7.5 - 2013-10-10 =
* Fix. Fix critical error with slider not working caused by easing plugin.
* New. Added ability to add a title to slider widget.
* Change. Modified easing plugin to v1.3.1.
* Change. Added minified version of easing plugin.

= 2.7.4 - 2013-10-01 =
* Fix. Fix dynamic height for templates.
* Change. Added RTL support and sanitize output in templates.

= 2.7.3 - 2013-09-28 =
* Fix. Fix issue on Default template where caption is not visible on images that are taller than the slider.
* Change. Returned slider auto height from sentinel to ratio for wider support and backward compatibility.
* Change. Updated screenshots for wordpress.org.

= 2.7.2 - 2013-09-27 =
* New! Added ability in Settings page to enable/disable templates.
* Change. Move settings page form to its own view file.

= 2.7.1 - 2013-09-23 =
* Added Width Management option. Three options available: Responsive (default), Full width, and Fixed width. Templates that support this feature are Dark, Default, Standard and Thumbnails.
* Added [Dark template](http://www.codefleet.net/cyclone-slider-2/templates/dark/) with RTL support.
* Standard template is now the selected template when creating new sliders.
* Moved Title and Description to Caption accordion in slide edit screen.
* Returned other shortcode options removed in 2.7.0. All shortcode options restored except template. Template can only be changed in admin.
* Fix caption text-align:left for templates standard, default and thumbnails along with RTL support.
* Updated language files

= 2.7.0 - 2013-09-19 - This is a major release = 
* Slider preview!
* Added YouTube and Vimeo slide types. Deprecated Video slide type.
* Added Standard template as de-facto template which has support for Image, YouTube, Vimeo, and Custom HTML slide types.
* Standard template supports RTL and uses pure CSS for buttons.
* YouTube and Vimeo videos will now pause when changing to a different slide when using the Standard template.
* Admin UI is now retina and [MP6](http://wordpress.org/plugins/mp6/) ready.
* Compacted template selection UI. Removed template thumbnail preview as a slider preview is now available in admin.
* Updated language files.
* Lots of new slider variables added for use in templates. Will update documentation soon.
* Removed other shortcode options except id. Example: [cycloneslider id="default"]
* [Pro version now available with many more features](http://www.codefleet.net/cyclone-slider-pro/).

= 2.6.4 - 2013-08-14 = 
* Bug fix for 2.6.3 where settings page stopped working.
* Minor fix for RTL.
* Added Persian translation by Javad.

= 2.6.3 - 2013-08-13 = 
* Made non-translatable texts translatable.
* Added RTL support for the admininistration screen.
* Change pin icon to media in the admin menu.
* Added Arabic translation. Special thanks to Hassan for this and the items above.
* Added function `cyclone_slider` for displaying slider in template files instead of using `do_shortcode`.
* Added button that links to a tutorial on how to [create your own template](http://www.codefleet.net/introduction-to-templates/).

= 2.6.2 - 2013-08-08 = 
* Reverted red screen options to default color.
* Fix bug with ugly old media gallery (pre 3.5).
* Added Italian translation from maxgx.
* Change greater-than to its character entity for `data-cycle-slides`.

= 2.6.1 - 2013-08-05 = 
* Fixed issue with Shortcodes Ultimate.
* Updated screenshots.

= 2.6.0 - 2013-08-04 = 
* Warning: Old templates will break in this version! You can either use the new templates or migrate the older templates. [Check this post](http://www.codefleet.net/pre-2-6-0-templates-migration/).
* Load scripts and styles normally as separate requests for better compatibility with other plugins and server setup. Removed template-assets.php which consolidates assets into a single request.
* Added cyclone slider settings page.
* Language files now loaded when using WPML.
* Added Get Codes metabox to easily grab the slider codes.
* Added Slideshow ID metabox to easily change the slider ID.

= 2.5.6 - 2013-07-30 = 
* Fix broken nextgen importer from last update.
* Refactor code for better template management in admin.

= 2.5.5 - 2013-07-25 = 
* Removed templates Black, Blue, and Myrtle from plugin's folder for better performance.
* Used get_posts instead of WP_Query when getting a slider to avoid filters that might cause conflict.

= 2.5.4 - 2013-07-20 = 
* Added Youtube template that pauses the video when slider is transitioning. 

= 2.5.3 - 2013-05-10 = 
* Bug fix for child themes where slider is not working

= 2.5.2 - 2013-04-26 = 
* Added template asset loader to get rid of the compiled css and js that are rewritten on the file system on every save
* Move template handling logic to its own class to be used by the template asset loader independently
* Removed upgrade notice

= 2.5.1 - 2013-03-29 = 
* Bug fix to allow small images to be inserted.
* Improved cyclone_settings.
* Improved slider not found message.
* Updated cycle 2 js files.
* Added plugin version to fix caching problem on JS and CSS.
* Added upgrade notice.

= 2.5.0 - 2013-03-21 - This is a major release = 
* More slide types to choose from: image, video (youtube and vimeo) and custom HTML.
* Added icons to the UI to indicate different slide types.
* Replaced cookies with localstorage to store UI status.
* Updated the templates to support the various slide types.
* Added resize and random options.
* Bug fix for fatal error when no GD library. Added gd_info check.
* Bug fix for js error on WP below 3.5 caused by the 3.5 media library object being undefined.
* Deprecated cycloneslider_thumb use cyclone_slide_image_url instead.
* Deprecated cycloneslider_settings use cyclone_settings instead.
* Deprecated cycloneslider_slide_settings use cyclone_slide_settings instead.
* Various UI fixes and code refactoring.

= 2.2.5 - 2013-02-23 = 
* Bug fix for 2.2.4

= 2.2.4 - 2013-02-22 = 
* Now compiles the template CSS and JS files instead of using template_redirect hook. This is to fix problems with some users reporting broken css and js.
* Minified CSS and JS for templates.
* Compiles needed CSS and JS only instead of loading all CSS and JS from all templates.
* Added template column to all slider screen.
* Updated language files

= 2.2.3 - 2013-02-14 = 
* Added option for random slide order on every page visit.
* Refactored some code.
* Added image count to all slider screen.

= 2.2.2 - 2013-02-05 = 
* Updated language files.
* Bug Fix. Post Type Switcher fix via jquery.
* UI Enhancement. Removed overflow for templates.
* Ignore image resize if slider dimension is equal to the image dimension.
* UI Enhancement. Decrease drag delay for slide sortables in editor.

= 2.2.1 - 2012-12-25 = 
* Added Cyclone Slider 2 widget. 

= 2.2.0 - 2012-12-24 = 
* Updated cycle 2 to latest version.
* Updated template selection interface to be more visual. A screenshot of each slider template is now shown.
* Added Tile Count and Tile Position for both slider and per-slide settings.
* Cleanup Quick Edit screen to hide unused user interface.
* Slide box titles can now be clicked to open and close the slide box.
* Removed drag icon from slide box title. Slide box can now be dragged by click-holding the slide title area.
* Updated template API functions.
* Updated plugin screenshot.
* Refactored various code parts.
* Added ability to add script.js in templates
* Added ability to add screenshot.jpg in templates.
* Updated templates.
* Added fix to preserved PNG transparency.
* Fix save routine to allow saving empty slides and to preserve order of slides after drag and/or deletion of slide.

= 2.1.1 - 2012-11-16 = 
* Fix for a code typo error

= 2.1.0 - 2012-11-16 = 
* Fix for slider not working when NextGEN 1.9.7 is active
* You can now import images from NextGEN

= 2.0.1 - 2012-11-09 = 
* Bug fix for hover pause

= 2.0.0 - 2012-10-28 = 
* Initial





== Upgrade Notice ==

= 2.8.4 - 2014-09-04 =
* Updated spanish language files
* Added compatibility with WP 4.0

= 2.8.3 - 2014-08-20 =
* Fix. Admin menu icon for WP 3.9+.
* Fix. Language files load path.

= 2.8.2 - 2014-01-10 =
* New. Added testimonial slide type. Now you can create testimonial sliders.
* New. Added support for testimonial slides in Dark and Standard templates.
* New. Added Spanish translation by Gabriel Gil.
* New. Added Serbo-Croation translation by Borisa Djuraskovic.
* Change. Added a few responsive tweaks in admin.css for the template selection area.
* Change. Removed unused codes. 

= 2.8.1 - 2014-01-02 =
* New. Added ability to disable related videos in YouTube slide.
* New. Slide title now appends the slide caption of there is one.
* New. MP6 color schemes. Added subtle cosmetic changes to UI depending on what admin color scheme was selected.
* Change. Made hide_non_active false only if using dynamic height and YouTube/Vimeo slides. For backwards compatibility with older templates.
* Change. Removed old problematic video slide.
* Fix. Fixed Vimeo error when URL fails to load.
* Fix. Fix for very long slide titles.
* Fix. Bug fix for PHP warning in template selection when template is unchecked in settings page.

= 2.8.0 - 2013-12-29 - This is a major release =
* New. Added support for YouTube, Vimeo and Custom slide types in Text template.
* New. Added support for YouTube and Vimeo slide types in Dark template.
* New. Added "Location" column in template selection panel.
* New. Added warning when a template is located in the currently active theme directory. It warns the user of potential deletion of the template when a theme is updated.
* New. Added template directory in wp-content/cycloneslider/. This is now the recommended directory to store custom or modified templates to survive update nukes.
* New. Added width_management to shortcode attributes.
* Change. hide_non_active is now always set to false for getBoundingClientRect to not return zero.
* Fix. Minor change for directory separator on active theme location.
* Fix. Fixed inacurate next slide height reading by using getBoundingClientRect() instead of outerHeight().
* Fix. Added check to fix PHP warning when Vimeo URL is blank.

= 2.7.7 - 2013-11-26 =
* New. Added ability to select multiple images to add as slides
* Change. Refactor code for template javascripts. Moved similar code into client.js

= 2.7.6 - 2013-10-13 =
* New. Added support for YouTube and Vimeo slide types in thumbnails template.
* New. Added ability to fetch thumbnails of videos from youtube.com and vimeo.com. The thumbnails template will use this to display the thumbnails in its pager.

= 2.7.5 - 2013-10-10 =
* Fix. Fix critical error with slider not working caused by easing plugin.
* New. Added ability to add a title to slider widget.
* Change. Modified easing plugin to v1.3.1.
* Change. Added minified version of easing plugin.

= 2.7.4 - 2013-10-01 =
* Fix. Fix dynamic height for templates.
* Fix. Fix video slide made it fluid.
* Change. Added RTL support and sanitize output in templates.

= 2.7.3 - 2013-09-28 =
* Fix. Fix issue on Default template where caption is not visible on images that are taller than the slider.
* Change. Returned slider auto height from sentinel to ratio for wider support and backward compatibility.
* Change. Updated screenshots for wordpress.org.

= 2.7.2 - 2013-09-27 =
* New! Added ability in Settings page to enable/disable templates.
* Change. Move settings page form to its own view file.

= 2.7.1 - 2013-09-23 =
* Added Width Management option. Three options available: Responsive (default), Full width, and Fixed width. Templates that support this feature are Dark, Default, Standard and Thumbnails.
* Added [Dark template](http://www.codefleet.net/cyclone-slider-2/templates/dark/) with RTL support.
* Standard template is now the selected template when creating new sliders.
* Moved Title and Description to Caption accordion in slide edit screen.
* Returned other shortcode options removed in 2.7.0. All shortcode options restored except template. Template can only be changed in admin.
* Fix caption text-align:left for templates standard, default and thumbnails along with RTL support.
* Updated language files

= 2.7.0 - 2013-09-19 - This is a major release = 
* Slider preview!
* Added YouTube and Vimeo slide types. Deprecated Video slide type.
* Added Standard template as de-facto template which has support for Image, YouTube, Vimeo, and Custom HTML slide types.
* Standard template supports RTL and uses pure CSS for buttons.
* YouTube and Vimeo videos will now pause when changing to a different slide when using the Standard template.
* Admin UI is now retina and [MP6](http://wordpress.org/plugins/mp6/) ready.
* Compacted template selection UI. Removed template thumbnail preview as a slider preview is now available in admin.
* Updated language files.
* Lots of new slider variables added for use in templates. Will update documentation soon.
* Removed other shortcode options except id. Example: [cycloneslider id="default"]
* [Pro version now available with many more features](http://www.codefleet.net/cyclone-slider-pro/).

= 2.6.4 - 2013-08-14 = 
* Bug fix for 2.6.3 where settings page stopped working.
* Minor fix for RTL.
* Added Persian translation by Javad.

= 2.6.3 - 2013-08-13 = 
* Made non-translatable texts translatable.
* Added RTL support for the admininistration screen.
* Change pin icon to media in the admin menu.
* Added Arabic translation. Special thanks to Hassan for this and the items above.
* Added function `cyclone_slider` for displaying slider in template files instead of using `do_shortcode`.
* Added button that links to a tutorial on how to [create your own template](http://www.codefleet.net/introduction-to-templates/).

= 2.6.2 - 2013-08-08 = 
* Reverted red screen options to default color.
* Fix bug with ugly old media gallery (pre 3.5).
* Added Italian translation from maxgx.
* Change greater-than to its character entity for `data-cycle-slides`.

= 2.6.1 - 2013-08-05 = 
* Fixed issue with Shortcodes Ultimate.
* Updated screenshots.

= 2.6.0 - 2013-08-04 = 
* Warning: Old templates will break in this version! You can either use the new templates or migrate the older templates. [Check this post](http://www.codefleet.net/pre-2-6-0-templates-migration/).
* Load scripts and styles normally as separate requests for better compatibility with other plugins and server setup. Removed template-assets.php which consolidates assets into a single request.
* Added cyclone slider settings page.
* Language files now loaded when using WPML.
* Added Get Codes metabox to easily grab the slider codes.
* Added Slideshow ID metabox to easily change the slider ID.

= 2.5.6 - 2013-07-30 = 
* Fix broken nextgen importer from last update.
* Refactor code for better template management in admin.

= 2.5.5 - 2013-07-25 = 
* Removed templates Black, Blue, and Myrtle from plugin's folder for better performance.
* Used get_posts instead of WP_Query when getting a slider to avoid filters that might cause conflict.

= 2.5.4 - 2013-07-20 = 
* Added Youtube template that pauses the video when slider is transitioning. 

= 2.5.3 - 2013-05-10 = 
* Bug fix for child themes where slider is not working

= 2.5.2 - 2013-04-26 = 
* Added template asset loader to get rid of the compiled css and js that are rewritten on the file system on every save
* Move template handling logic to its own class to be used by the template asset loader independently
* Removed upgrade notice

= 2.5.1 - 2013-03-29 = 
* Bug fix to allow small images to be inserted.
* Improved cyclone_settings.
* Improved slider not found message.
* Updated cycle 2 js files.
* Added plugin version to fix caching problem on JS and CSS.
* Added upgrade notice.

= 2.5.0 - 2013-03-21 - This is a major release = 
* More slide types to choose from: image, video (youtube and vimeo) and custom HTML.
* Added icons to the UI to indicate different slide types.
* Replaced cookies with localstorage to store UI status.
* Updated the templates to support the various slide types.
* Added resize and random options.
* Bug fix for fatal error when no GD library. Added gd_info check.
* Bug fix for js error on WP below 3.5 caused by the 3.5 media library object being undefined.
* Deprecated cycloneslider_thumb use cyclone_slide_image_url instead.
* Deprecated cycloneslider_settings use cyclone_settings instead.
* Deprecated cycloneslider_slide_settings use cyclone_slide_settings instead.
* Various UI fixes and code refactoring.

= 2.2.5 - 2013-02-23 = 
* Bug fix for 2.2.4

= 2.2.4 - 2013-02-22 = 
* Now compiles the template CSS and JS files instead of using template_redirect hook. This is to fix problems with some users reporting broken css and js.
* Minified CSS and JS for templates.
* Compiles needed CSS and JS only instead of loading all CSS and JS from all templates.
* Added template column to all slider screen.
* Updated language files

= 2.2.3 - 2013-02-14 = 
* Added option for random slide order on every page visit.
* Refactored some code.
* Added image count to all slider screen.

= 2.2.2 - 2013-02-05 = 
* Updated language files.
* Bug Fix. Post Type Switcher fix via jquery.
* UI Enhancement. Removed overflow for templates.
* Ignore image resize if slider dimension is equal to the image dimension.
* UI Enhancement. Decrease drag delay for slide sortables in editor.

= 2.2.1 - 2012-12-25 = 
* Added Cyclone Slider 2 widget. 

= 2.2.0 - 2012-12-24 = 
* Updated cycle 2 to latest version.
* Updated template selection interface to be more visual. A screenshot of each slider template is now shown.
* Added Tile Count and Tile Position for both slider and per-slide settings.
* Cleanup Quick Edit screen to hide unused user interface.
* Slide box titles can now be clicked to open and close the slide box.
* Removed drag icon from slide box title. Slide box can now be dragged by click-holding the slide title area.
* Updated template API functions.
* Updated plugin screenshot.
* Refactored various code parts.
* Added ability to add script.js in templates
* Added ability to add screenshot.jpg in templates.
* Updated templates.
* Added fix to preserved PNG transparency.
* Fix save routine to allow saving empty slides and to preserve order of slides after drag and/or deletion of slide.

= 2.1.1 - 2012-11-16 = 
* Fix for a code typo error

= 2.1.0 - 2012-11-16 = 
* Fix for slider not working when NextGEN 1.9.7 is active
* You can now import images from NextGEN

= 2.0.0 =
* Initial. If you are using Cyclone Slider (version 1) deactivate it first before activating Cyclone Slider 2
