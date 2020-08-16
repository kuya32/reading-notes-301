# Read: 07 - APIs continued

## How I explained REST to my brother

- Roy Fielding
  - Creator of first web server, HTTP - tells browser what protocol to use
  - His name is on the specification for the protocol that is used to get pages from servers to your browser
- **HTTP** is capable of describing the location of something anywhere in the world from anywhere in the world.
  - think of it like GPS coordinates for knowledge and information
- Whole wide web is built on an architectural style called **“REST”** which provides a definition of a “resource”, which is what those things point to
- URLs tell the browser that there's a concept somewhere. A browser can then go ask for a specific representation of the concept
  - browser asks for the web page representation of the concept.
- “Web Services” or "APIs". The basic concept is that machines could use the web just like people do.
- We eventually want machines talking with each other to get what we want faster and easier
  - Machines tell each other where things are by the URL which all these systems tell each other about each other’s nouns
- **“polymorphism”** - different nouns can have the same verb applied to them.
  - GET, PUT and DELETE
    - When you go to a web page, the browser does an HTTP GET on the URL you type in and back comes a web page.
- HTTP is actually a general purpose protocol for applying verbs to nouns.
- Machines only care about data, every URL would have a human readable and a machine readable representation.
- “Polymorphism” verbs:
  - GET -  every URL would have a human readable and a machine readable representation.
  - POST -  If one system needs to add something to another system
  - PUT -  If a system wants to replace something in another system
  - PATCH -  to do a partial update
- Now we have flashy tools to communicate between machines

[Back to README](README.md)
