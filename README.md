# Archive Blocked Keywords

* This will be listed keywords to be auto blocked for file names using to block the files uploaded to Telegram Archive Website.
* Keyword List [Here](https://github.com/PBhadoo/Archive-Blocked-Keywords/blob/main/blocklist.js)

## JS Function used, Improve it if you can

````
var blocked_keywords = ["keyword1", "keyword2"]

for (var i = 0; i < blocked_keywords.length; i++) {
    if (name_of_file.toLowerCase().includes(blocked_keywords[i].toLowerCase())) {
        console.log("Blocked keyword found: " + blocked_keywords[i]);
        return new Response("OK", {
            status: 200,
            headers: {
                "content-type": "application/json",
            },
        })
        break; // Stop searching for other blocked keywords
    }
}
````
