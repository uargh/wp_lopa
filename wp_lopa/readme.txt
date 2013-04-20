=== Logarithmic Pagination ===
Contributors: uargh
Tags: pagination, navigation, archives, categories, search, tags, pages
Requires at least: 3.0.1
Tested up to: 3.5.1
Stable tag: 0.1
Plugin URI: http://www.k308.de/wp/logarithmic-pagination
Author URI: http://blog.k308.de
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

This plugin inserts pagination based on logarithmic calculation for a more evenly distributed link-juice.

== Description ==

This will give you an advanced pagination to distribute your link-juice more evenly across your paginated paged. It also provides a better choice of navigation to the user tio explore and find your content.

You can turn the pagination on/off seperately for:

*	homepage
*	search results
*	category archives
*	date archives
*	tag archives

You can also choose if you want it to be displayed before and/or after the loop content.

The plugin is currently available in English and German. If you want to help translate it, just write me an email. Help is much appreciated!

For more information visit the [plugin website](http://labs.k308.de/wp/logarithmic-pagination "Logarithmic Pagination plugin page").

== Installation ==

1. Unzip wp-lopa.zip.
1. Upload `wp-lopa` to the `/wp-content/plugins/` directory
1. Activate the plugin through the `Plugins` menu in WordPress
1. Change Settings on `Settings` -> `Log. Pagination`
1. Remove original pagination code from template files
1. Add some CSS to make it all pretty. To make it easier here is some sample-code:

.paging-navigation ul {
	list-style: none;
}

.paging-navigation li {
	float: left;
}

.paging-navigation .current {
}

.paging-navigation .paginate_link {
}

.paging-navigation .prev {
}

.paging-navigation .next {
}

Here is some sample HTML output:

<nav role="navigation" id="pages_bottom" class="site-navigation paging-navigation">
	<h1 class="assistive-text">Post navigation</h1>
	<ul>
		<li><a href="?paged=2" rel="prev" class="prev"><span class="paginate_link">Previous</span></a></li>
		<li><a href=""><span class="paginate_link">1</span></a></li>
		<li><a rel="prev" href="?paged=2"><span class="paginate_link">2</span></a></li>
		<li><span class="current">3</span></li>
		<li><a rel="next" href="?paged=4"><span class="paginate_link">4</span></a></li>
		<li><a href="?paged=5"><span class="paginate_link">5</span></a></li>
		<li><span class="seperator">..</span></li>
		<li><a href="?paged=7"><span class="paginate_link">7</span></a></li>
		<li><span class="seperator">..</span></li>
		<li><a href="?paged=11"><span class="paginate_link">11</span></a></li>
		<li><span class="seperator">..</span></li>
		<li><a href="?paged=19"><span class="paginate_link">19</span></a></li>
		<li><span class="seperator">...</span></li>
		<li><a href="?paged=35"><span class="paginate_link">35</span></a></li>
		<li><span class="seperator">..</span></li>
		<li><a href="?paged=42"><span class="paginate_link">42</span></a></li>
		<li><a href="?paged=4" rel="next" class="next"><span class="paginate_link">Next</span></a></li>
	</ul>
</nav>


== Frequently Asked Questions ==

= What about foo bar? =

I don't know either.

== Screenshots ==

1. This screen shot show an example of this plugins output.
2. This screen shot shows the Settings page.

== Other Notes ==

= Credits =

This plugin is based on the idea found in the following (German) article by Nikolas Schmidt-Voigt: [Webseitenstruktur und Paginierung für SEO](http://www.kawumba.de/webseitenstruktur-und-paginierung-fuer-seo/ "Logarithmic Pagination plugin page") & a 
[discussion](http://stackoverflow.com/questions/7835752/how-to-do-page-navigation-for-many-many-pages-logarithmic-page-navigation "") on stackoverflow.

== Changelog ==

= 0.1 =
This is the initial version.
Features:
1. Seperately control pagination before and after the loop
1. Seperately control pagination on homepage, category archives, date archives, tag archives and search-results
1. Control and set text for `Previous` and `Next` links

== Upgrade Notice ==

= 0.1 =
This is the initial version.