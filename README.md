# links-webpage-demo
A Linktree-type webpage that is built using HTML, JavaScript, and JSON.

## Before getting started
- This implementation requires JavaScript to be allowed on the client's (end user's) machine. Because of this, it is recommended to include a `<noscript>` banner/text in case JavaScript is not turned on.
- Local testing may result in CORS policy errors. To resolve these issues, host the files on a [local server](https://github.com/samharp/localserve-batch).
- Provided CSS is not required for implementation and is purely for demonstration purposes.

## How it works
The included JavaScript looks at the `links.json` file and creates a link element for each JSON object. The JavaScript runs down the list of objects and creates them in order they appear in the JSON. You can move the HTML Template and container wherever you like on the HTML page, as long as they keep their custom attributes (i.e. `data-links-container`, `data-link-row`, etc.).

## What's included in each link?
By default, each JSON element contains the link text (`label`) and the link path (`href`). This can be modified to include additional data, such as CSS classes, IDs, custom attributes, and more.

__If additional data is included in JSON, ensure that each object contains the same key-value pair. For example:__

```
{"linkItems": [
  {"label": "Portfolio", "href": "https://sammyharper.com", "style": "portfolio_link"},
  {"label": "Terrabyte", "href": "https://terrabyte.eco", "style": "terrabyte_link"}
]}
```
