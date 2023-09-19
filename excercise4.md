# Excercise 4

sequenceDiagram
    User->>Browser: Enters site URL
    loop 
    Browser->>Server: Sends a HTTP GET Request
    Server ->> Browser: Returns site files
    Browser ->> User: Runs JavaScript and shows the user the site's content
    User ->> Browser: Interacts with the site by submitting a new note
    Browser ->> Server: Sends a HTTP Post request
    Server ->> Browser: Redirects the browser to /notes route
    Browser ->> Server: Sends HTTP GET Request <br/>
    end
