# Excercise 4

flowchart TD
User -- Enters URL --> Browser
Browser -- Sends a GET request --- Server
Server -- Returns --> files
Submit -- Form sends browser to --> Server
subgraph files[App Files]
HTMl -- loads --> CSS & JavaScript
JavaScript --> Render[Render the site]
end
files -- Rendered site contains a --> Form
Form --  Contains action --- Submit
User --> Submit
