# Welcome to Cherry

Purposed of enclosed files:
manifest.json: contains all extensions used in the project, json formatted file
background scripts (background.js): "running in the background of the chrome browser" event listeners. Background scripts must be added to the manifest under the "background" field
``` 
"background" : {
    "scripts" : [ "background.js" ],
    "persistent" : false
  }
```
content scripts: interact with the DOM. These can read pages that the broswer visits, and can make changes to them and pass along information to the extension.
popup (popup.js): view, starts background page by calling runtime.getBackgroundPage .
options page: 


Debugging Chrome extensions: ``` https://developer.chrome.com/extensions/tut_debugging```

1. go to ```chrome://extensions```
2. click load unpacked, and select project to debug. 3 buttons should pop up: Details, Remove, Errors
- Errors allows you to see errors in the background scripts, check stack trace

