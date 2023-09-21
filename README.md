# Description

Basic countdown timer using craft cms custom css/js and the craft craft cms calendarize plugin.

# Requirements

JSON data with a unix timestamp for the time you're counting down to. Sample:

    {"next_timestamp":1330043400,"next_title":"Samson","next_description":"Emotions That Take Strong Men Down"}

"next_title" and "next_description" are completely optional.  If you choose not to use them, you can remove references to them in the sample HTML, CSS, and JS.

# Notes

1. Some browsers (like Chrome) are big fans of making AJAX calls to local files.  So if you want to test out this code as-is, just fire up a Python server and point your browser to ```http://localhost:8000```

        $ cd /my-project-path/
        $ python -m SimpleHTTPServer

2. The sample JSON file (data.json) includes a timestamp that may be old.  If you load this all up to preview it, make sure you change the timestamp to something in the future. (Not neccessary if using data.json.twig in craft as it will automatically update.)
