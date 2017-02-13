# cosi-nav
A simple component for the navigation list at the top of most COSI webpages

## Installation
To use this component on a website, copy the following files into the new site's
directory:

* fetch.js: The polyfill to enable window.fetch on all browsers
* cosi-nav.js: The file to fetch and generate the new files

Next, add the following additions to your site:

```html
<html>
	<head>
		<!-- The site agnostic styling for the cosi-nav element -->
		<link rel="stylesheet" href="https://dubsdot.cosi.clarkson.edu/cosi-nav.css">

		<!-- The fetch polyfill. Change the src to wherever you store js files -->
		<script src="/js/fetch.js"></script>

		<style>
			:root {
				/* Change these two variables to make the navbar
				   fit with the design of the website */
				--background-color: black;
				--text-color: white;
			}
		</style>
	</head>

	<body>
		<!-- The actual element that will be filled when the page loads -->
		<cosi-nav></cosi-nav>

		<!-- The script which fetches the JSON and renders the navbar -->
		<script src="/js/cosi-nav.js" defer></script>
	</body>
</html>
```

## COSI-Nav modification
If there is a new website that is going to be added to the list, change the [cosi-nav.json](cosi-nav.json)
file, commit it, and then pull the changes down in the directory for Dubsdot's webpage (dubsdot:/var/www/html/).