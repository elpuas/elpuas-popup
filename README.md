# elpuas-popup
WP Plugin - Shortcode to open a link inside a popup browser window

Add popups to your site. Add links to pages/posts via a shortcode which will be opened in a popup browser window.

== Description ==

This plugin allows you to enter a shortcode to add links to pages/posts which will be opened in a popup window. The only options in Alligator popup are entered in the shortcode, so there is no admin page for this plugin.

#### Shortcode:
Add a popup shortcode where you would like a link to appear within your post or page text. The shortcode has parameters for url, height and width and should be in the format:

`[popup url="http://elpuas.com" height="300" width="300" scrollbars="yes" alt="popup"]Link Text[/popup]`

Include your own Link Text and values for the url the width & height of the popup, and the alt text fot the link.

If no values are entered for the alt text and the height and width, defaults of 400px are used for the width & height of the popup window.

Scrollbars are enabled by default and will show if the scrollbars parameter is not added to the shortcode. If you do not want scrollbars on your popup window, add the scrollbars parameter with the value "no" to the shortcode: `scrollbars="no"`

If no value is entered for the alt text, an empty alt tag will be used in the link.

#### HTML Link:
Instead of using the shortcode you can include your link in the format:
`<a href="http://elpuas.com" class="popup" data-height="300" data-width="300" data-scrollbars="0" alt="my link text">Link Text</a>`

This might be useful in a text widget, or you can build the link in a template file of your theme.

#### Note:
If you are using any other plugin (or a theme) that uses a shortcode with the name 'popup', you will not be able to use this plugin. This is not because of any shortcoming in this plugin, but because shortcodes such as those to create popup links should always be implemented in a plugin not a theme.

On mobile devices such as iPads which don't use browser windows, the link will open in a new tab.

