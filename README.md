I don't use this anymore, I use [Redirector](https://addons.mozilla.org/en-US/firefox/addon/redirector/) which is a general purpose version of this addon.

My first redirect rule which does what this addon did, is this (exported from Redirector):

```json
{
    "createdBy": "Redirector v3.2.1",
    "createdAt": "2019-07-07T06:22:56.000Z",
    "redirects": [
        {
            "description": "YouTube -> Invidio.us",
            "exampleUrl": "https://www.youtube.com/embed/9HimzZ6QG2o",
            "exampleResult": "https://invidio.us/embed/9HimzZ6QG2o",
            "error": null,
            "includePattern": "(.*\\.)youtu(be.com|\\.be)/(.*)",
            "excludePattern": "",
            "patternDesc": "Redirect Youtube videos to Invidious",
            "redirectUrl": "https://invidio.us/$3",
            "patternType": "R",
            "processMatches": "noProcessing",
            "disabled": false,
            "appliesTo": [
                "main_frame",
                "sub_frame"
            ]
        }
    ]
}
```
