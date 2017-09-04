=== Facebook Instant Articles for WordPress Plugin - WP Native Articles Pro ===

Contributors: ozthegreat
Donate link: https://wp-native-articles.com
Tags: facebook, instant articles, facebook instant articles, mobile, speed, optimize, performance
Requires at least: 4.0
Tested up to: 4.8.1
Stable tag: 1.2.5
Requires PHP: 5.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Text Domain: wp-native-articles
Domain Path: /languages

Easy Facebook Instant Articles Plugin for your WordPress site with better content parsing and advanced features.

== Description ==

**Major Updates**

- 1.2.5 - Specify different content for your Instant Article
- 1.2.2 - WP Bakery Visual Composer Support

A better implementation of Facebook Instant Articles for WordPress.

Only available in the Facebook mobile app, Instant Articles are a pre-loaded, super fast, and optimized version of your regular articles. Boasting some impressive stats (10x faster, 20% more reads, 70% less abandonment) they have quickly become a must for every publisher.

**How it works**

After installation and setup this plugin auto generates an instant article version for each of your WordPress articles. The article's regular HTML is parsed and converted to correct Facebook Instant Article markup which is then submitted to Facebook via an RSS feed. Anytime your article is then viewed using the Facebook mobile app it will load the pre-cached, super fast, optimized version. When the article is shared or posted its instant status will also be denoted by the lightning symbol in the corner.

[Read more about Instant Articles from the official documentation](https://developers.facebook.com/docs/instant-articles)

**Content Parsing**

A large part of the complexity of integrating Facebook Instant Articles is the rigorous content structure imposed. Due to the WYSIWYG editor and the plethora of plugins and themes available, WordPress content tends to be rather unstructured. Most of the current Facebook Instant Article plugins don't really take account of this and either produce invalid content or strip parts out. This plugin is a concentrated effort to correctly format any WordPress content it could possibly come across. You can read more about the challenges and solutions faced when parsing unstructured content on our [Instant Articles blog](https://wp-native-articles.com/blog/formatting-wordpress-html-content-instant-articles/?utm_source=fplugin&utm_medium=readme).

> **PRO Version**
>
> [WP Native Articles Pro](https://wp-native-articles.com/?utm_source=fplugin&utm_medium=readme-a) comes with full [Facebook Instant Articles API](https://wp-native-articles.com/?utm_source=fplugin&utm_medium=readme-b#features) integration and has more advanced features such as:
>
> * **Full API integration**
> * **Manage Articles** Publish, unpublish and manage Instant Articles directly from the WordPress post page.
> * **Live Sync** Instant Articles synced instantly from WordPress, no waiting for FaceBook to scrape the RSS feed.
> * **Individual Sync** Only make posts of your choosing Instant Articles
> * **Article Status** Errors & import status for your Instant Articles displayed live in every article.
> * **Instant Articles Analytics** Individual and aggregated site overview analytics, broken down by device and date.
> * **Premium support**
>
> Check out the Pro version at [https://wp-native-articles.com/](https://wp-native-articles.com/?utm_source=fplugin&utm_medium=readme-c).

**Future**

Features planned for the near future.

* Placement manager (ads, related articles, anything)
* Sync all your old articles
* Embed WordPress Comments
* Advanced stats & weekly roundup email
* CLI & API integration

== Installation ==

1. Upload *wp-native-articles-pro* to the */wp-content/plugins/* directory
2. Activate the plugin through the Plugins menu in WordPress
3. Go to *Native Articles* in the admin sidebar to manage settings
4. When you're ready submit your feed to Facebook. [Full instructions](https://developers.facebook.com/docs/instant-articles/publishing/setup-rss-feed)

== Upgrade Notice ==

Intentionally left blank

== Frequently Asked Questions ==

= Where can I find the support documentation? =

All documentation is available at [docs.wp-native-articles.com](http://docs.wp-native-articles.com). It is a work in progress so please bear with us.

= Does it support Branded Content? =

Yes. Individual articles can be setup as branded. The author details are used and displayed on the Instant Article.

= Does it support Ads & Analytics? =

Yes. Both can be added on a global level or overridden for individual articles.

= I use ACF or Meta Fields to display some content. Are these supported? =

They won't automatically be added to the Instant Articles unfortunately. However, they should be easy enough to add as
not only are there hooks galore in the plugin but the Instant Article templates can be overridden in your own theme or plugin.

= Does it play well with other plugins? =

Yes, extremely well. We've tested loads of popular plugins that embed content and built in support for Yoast, Co-Authors-Plus, Visual Bakery and Playbuzz to name a few.
If you find any that don't work or that we've missed please let us know and we'll be sure to fix them.

= Is there a road map? =

Yep. It can be found on our [instant articles roadmap page](https://wp-native-articles.com/roadmap/?utm_source=fplugin&utm_medium=readme-d).

= Does it support WordPress Multisite? =

Yes it does. There's a management panel in the Network Admin sidebar menu.
It can be used to copy settings from one blog to another and set a default blog
to inherit settings from when new blogs are created.

= Does it support custom post types? =

Yes. The RSS feeds defaults to posts but custom post types can be specified by pass in query parameters. More information can be [found here](http://docs.wp-native-articles.com/article/44-custom-post-types)

= Is it multilingual compatible? =

Yes. All text strings use the WordPress i18n translation functions. If you'd like to help translate the plugin we'd love to hear from you!

= Does it work for multi-language sites? =

Yes. If you're using the WPML plugin it will generate a combined feed of all languages by default or you can pass in query parameters to specify which languages you'd like.

= What's the minimum PHP version required? =

It has the same requirements as WordPress, so PHP >= 5.2.4.

= I've found a bug? I have a feature request? =

Excellent. We'd love to hear from you. All support for the free plugin is done
through the WordPress support forum found on the Plugin download page.

== Screenshots ==

1. Global options.
2. Global styling options.
3. RSS Feed options.
4. Post options overrides.
5. Post styling overrides.
6. Content & related articles overrides.
7. Multisite options page.

== Changelog ==

= 1.2.5 =
* Feature. Post content override. You can now specify different content for IA
* Feature. Add [wpna hide=''][/wpna] shortcode for when you want to hide content from IA
* Feature. You can now manually specify related posts
* Feature. Removes paragraphs that only contain &nbsp;
* Feature. Prepare plugin for translation + fix spelling errors
* Feature. Better parsing for theme.co Pro & X
* Feature. Faster method for checking if images exist
$ Feature. Selective sync individual posts
* Fix. Bug with ChartJs that caused conflicts with some other JS libs
* Fix. Bug with post analytics not being returned correctly
* Fix. Better compatibility with older versions of Newmag theme
* Fix. Post status error table now works on mobile

= 1.2.4 =
* Feature. Add initial support for WP Quads
* Feature. Add initial support for theme.co Pro & X
* Feature. Better rules when dealing with shortcodes in posts
* Fix. 32bit support. Don't use absint for super large numbers
* Fix. Allow some html tags in the excerpt
* Fix. Development mode via the API didn't always work
* Fix. Stop publishing auto-drafts
* Fix. Pro Auto-updater now uses strict SSL verify
* Fix. Occasional encoding error. Punctuation no longer appears as ã
* Fix. Missing op-interactive tag in the Newsmag compatibility
* Fix. Ignore <!--nextpage--> tags

= 1.2.3 =
* Feature. Choose which articles you want published as Instant Articles
* Feature. Support for GitHub gist embeds added
* Feature. Support for &lt;pre&gt; & &lt;code&gt; tags added
* Feature. YouTube & Vimeo videos added through FV Player Plugin now supported
* Feature. Support for Newsmag theme Video posts added
* Fix. In-page links now removed
* Fix. Remove images less than 1024 bytes
* Fix. Bug affecting images wrapped in links
* Fix. Bug where some elements wouldn't get removed

= 1.2.2 =
* Feature. Support for Visual Bakery (beta)
* Feature. Optionally show subtitle, kicker, authors & media in the article header
* Feature. Add Facebook ad density option
* Feature. Add Facebook recirculation ad option
* Fix. Embedding other WordPress posts from your site now works
* Fix. Using embed code from Twitter & Instagram directly now works

= 1.2.1 =
* Fix. Bug with [gallery] images

= 1.2.0 =
* Feature. Now supports custom post types in the RSS feed
* Feature. Article kicker doesn't display if the category is 'uncategorized'
* Fix. Article kicker now displays the category name instead of the category slug
* Fix. Bug when a Page ID wasn't correctly set
* Fix. Bug with screen metaboxes
* Fix. Ensures whole post is displayed when <!--MORE--> tag is present
* Fix. [gallery] shortcodes should now show correctly

= 1.1.6 =
* Feature. Can now use dynamic date variables in Copyright & Credit fields
* Feature. Shows a warning if the API doesn't have the correct permissions
* Feature. Shows any API errors
* Fix. API flow now has better checking
* Fix. API now works with 2.8
* Fix. Date validation for PHP <= 5.3 now works

= 1.1.5 =
* Feature. Notify if a template is being overridden
* Fix. Ads script was sometimes being escaped
* Fix. Now works with the new Facebook API
* Fix. Saving API login settings sometimes wouldn't work

= 1.1.4 =
* Fix. Post settings sometimes override global defaults when they shouldn't

= 1.1.3 =
* Feature. Show warning if options have been overridden using hooks
* Fix. Error blocking the Screen Options tab on the post page
* Fix. Error sanitizing post options

= 1.1.2 =
* Feature. Image title & caption styling options. Global + post override
* Feature. Background CRON post api syncing
* Feature. Now 100% WordPress & WordPress VIP standards compatible
* Feature. Update to Facebook API v2.8
* Feature. Overridden templates can now be in a folder rather than top-level
* Fix. Post instant articles stats not showing (disconnect then re-connect your Facebook account)
* Fix. Post tabs not aligning
* WordPress 4.7.3 compatibility

= 1.0.9 =
* Fix Infogram embeds

= 1.0.8 =
* WordPress 4.7.1 compatibility
* Auto updater bug fix

= 1.0.7 =
* Auto updater fixes

= 1.0.6 =
* PHP 5.2 compatibility
* Update auto updater to fix caching issues

= 1.0.5 =
* Fix PHP <= 5.5 error

= 1.0.4 =
* Fix error when deleting an article via the API and Facebook isn't connected
* Fix error in image captions with non alphanumeric entities

= 1.0.3 =
* WordPress 4.7 compatibility
* Speed improvements for locating attachment IDs

= 1.0.2 =
* Fix for images using HTML5 markup
* Take account of captions when removing images
* Readme corrections

= 1.0.1 =
* Readme corrections

= 1.0.0 =
* Plugin released
