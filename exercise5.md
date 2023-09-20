# Excercise 5

sequenceDiagram
    User->>Browser: Enters site URL
    Browser->>Server: Sends a HTTP GET Request
    Server ->> Browser: Returns site files
    Browser ->> User: Runs JavaScript and shows the user the site's content
    User ->> Browser: Interacts with the site by submitting a new note
    Browser ->> Server: Sends an HTTP Post request
    Server ->> Browser: Sends a response
    Browser ->> User: Runs code using the response and renders updated note list<br/>without the need of reloading the site.
