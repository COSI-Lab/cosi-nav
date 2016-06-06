# cosi-nav
A simple web component for the navigation list at the top of most COSI webpages

## Usage
To use this web component on a website, download the webcomponents polyfill
from [webcomponents.org](http://webcomponents.org) under the Polyfills section.
Then import webcomponents.min.js into the head section of the webpage and
import the cosi-nav html file in the head section as well as such:

```html
<link rel="import" href="/path/to/components/cosi-nav.html">
```

Then place the cosi-nav tag at the top of a webpage:

```html
<!-- Head -->
<body>
	<cosi-nav></cosi-nav>
	<!-- Rest of file -->
```

Edit the css in cosi-nav.html to style it.

## Support

Web components with the polyfill support all mobile browsers, Chrome, Firefox,
Safari 7 and up, and IE11 and up.
