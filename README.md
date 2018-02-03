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

### config: internallinkHideDisplayText

Set to true, to hide 'Display text' field and operate with search field only. (CKEditor config.js):

    ````js
    config.internallinkHideDisplayText = true
    ````

