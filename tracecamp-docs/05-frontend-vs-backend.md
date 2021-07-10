# Frontend vs Backend

## Frontend

The frontend deals with loading the webpage in the browser. The frontend is also referred to as client side. Webpages primarily made with:

- **HTML** - the skeleton and data
- **CSS** - the design and styling
- **JavaScript** - interactivity and programming logic

We will learn more about HTML, CSS, and JavaScript in upcoming lessons. Frontend concerns include loading content that the webpage needs, such as images, fonts, and requests for additional data. We can build webpages without a backend.

## Backend

The backend is everything that happens on the server. The backend is also referred to as the server side. Some backends can be very complex, involving multiple databases, servers, data processes, and backups. Some backends can be very simple and return static (unchanging) files, like images.

Backend concerns include everything outside of the browser. When a webpage makes additional requests to the server, the server should process the request and return the data in a response.

## Loading a webpage

For example, let’s look at [sidebar.io](https://sidebar.io/), a popular blog for designers. Let’s think about what happens when you load the website in your browser:

- Your computer connects to the internet through your internet service provider
- You send a request to sidebar.io
- Domain name servers translate sidebar.io into an IP address
- You send an http request to that IP address with the default http port 80
- The server is listening on port 80 for any incoming requests
- The server receives your request
- The server makes a request to the database
- The database, perhaps on a difference machine, returns the appropriate data
- The server builds your webpage with up-to-date data
- The server sends the webpage in a response back to your browser
- The browser loads and displays the webpage
- The webpage makes additional requests for images, fonts, and other data it needs

Not all websites follow the same steps. They vary depending on the website needs and optimizations.

## Curriculum

In our curriculum, a majority of our code will be frontend code. We will be learning React.js, which is one of the big three frontend libraries/frameworks. HTML, CSS and JavaScript are all frontend languages. In recent years, JavaScript can also run on the server using Node.js.

When communicating with 3rd party APIs later in the course, we will not be building backends. However, we will briefly experiment with our own server side code in the context of serverless functions.

## Practice

N/A

## Optional

Always be thinking about whether the code you are writing is in the frontend or backend. Build a mental model to think about what happens when your webpage loads.

## [Next lesson →](./06-html.md)
