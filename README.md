# Logarithmic Pagination Plugin for Wordpress

This will give you an advanced pagination to distribute your link-juice more evenly across your paginated paged. It also provides a better choice of navigation to the user tio explore and find your content.

## Installation

1. Unzip wp-lopa.zip.
1. Upload `wp-lopa` to the `/wp-content/plugins/` directory
1. Activate the plugin through the `Plugins` menu in WordPress
1. Change Settings on `Settings` -> `Log. Pagination`
1. Remove original pagination code from template files
1. Add some CSS to make it all pretty. To make it easier here is some sample-code:

```css
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
```

Here is some sample HTML output:

```html
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
```

A Wordpress Plugin for better Pagination