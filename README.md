# ckeditor-internal-link

This plugin allows you to edit links with internal-links along with Autocomplete.

## Installation

 1. Download plugin
 
 2. Extract to plugins directory in ckeditor

 3. Add the plugin to CKEditor (config.js):

    ````js
    config.extraPlugins = 'internallink';
    ````

## How to use
If everything is ok, a Internal-link icon should appear on the CKEditor toolbar, in links section. Click on it.


### config: internallinkServiceURL (Required)
 
  Service URL to be invoked to fetch links and it's titles. (CKEditor config.js).
  
 ````js
 config.internallinkServiceURL = "https://www.nak-west.de/api/plugin/ckeditor/search";
 ````

#### Request params
  Service URL will be invoked with 2 params 'q'(search query) and 'c'(URL).
  
#### Response format
  Response MUST be an array of results with 'title' and 'link' details in it

 ````js
 {
	"results": [
		{
			"title": "",
			"link: ""
		}, {
			"title": "",
			"link: ""
		},
		.
		.
		.
		{
			"title": "",
			"link: ""
		}
	]
 }
 ````

### config: internallinkHideDisplayText
 
  Set to true, to hide 'Display text' field and operate with search field only. (CKEditor config.js):

 ````js
 config.internallinkHideDisplayText = true
 ````

