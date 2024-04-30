# Rendering:

Rendering converts the code you write into user interfaces. React and Next.js allow you to create hybrid web applications where parts of your code can be rendered on the server or the client.

# Fundamentals of Rendering:

There are three fundamentals concepts of Rendering,

1. Rendering Environments.
2. Request-Response LifeCycle.
3. Network Boundary.

## 1. Rendering Environments:

There are two Rendering Environmennts.

### • Clients

The clients refer to the browser on a user's device that sends a request to a server for your application code.</p>

### • Server

The server refers to a computer in a data center that store your code.

![alt text](image.png)

---

## 2. Request Response LifeCycle:

### • User Action:

The user interacts with your Next.js application, either by typing a URL into their browser or clicking a link. This triggers an HTTP request to the Next.js server.

### • HTTP Request:

The client sends an HTTP request to the server that contains necessary information about what resources are being requested, what method is being used (e.g. GET, POST), and additional data if necessary.

### • Server:

The server processes the request and responds with the appropriate resources. This process may take a couple of steps like routing, fetching data, etc.

### • HTTP Response:

An HTTP response is the server's reply to your web request. It includes a status code (success or error), and the requested resources like HTML, CSS, and JavaScript to build the web page you see.

### • Client:

The browser breaks down received data (HTML, CSS, JS) into its building blocks, then assembles them to create the web page you see.

### • User Action:

Once the user interface is rendered, the user can interact with it, and the whole process starts again.

---

## 3.Network Boundary:

---

# Types Of Rendering

There are two types of rendering Client side renderng & Server side Rendering.

## Client side Rendering:

Client side rendering refers to the process where our application is rendered on client side, meaning that the data is delevered from the server to client side in to HTML, then the page is show to the user.

<img src="image-1.png" width="300" height="200">

This image illustrates the process of loading a website in a browser:

##### 1. User requests a browser:

A user initiates a request to open a web browser.

##### 2. Browser requests a server:

The browser sends a request to the server to retrieve the content of a particular web page.

##### 3. Server sending an HTML file with JS:

The server responds to the browser's request by sending back an HTML file along with JavaScript (JS) code. This HTML file contains the basic structure of the web page, while the JavaScript adds interactivity and functionality to the page.

##### 4. Browser downloads HTML file (loading 10%):

The browser begins downloading the HTML file sent by the server. The loading progress is indicated as 10%.

##### 5. Browser downloads CSS & JS (loading 50%):

While the HTML file is being downloaded, the browser also starts downloading any CSS and JavaScript files referenced in the HTML. These files are necessary for styling the web page and adding interactivity. The loading progress for CSS and JS files is indicated as 50%.

##### 6. Browser loads whole website (loading 100%):

Once all the necessary files (HTML, CSS, and JS) are downloaded, the browser starts rendering the entire website. As the rendering process progresses, the loading progress reaches 100%, indicating that the website is fully loaded and ready for interaction.

### DisAdvantages of CSR:

- When JavaScript code is sent from the server, it significantly impacts SEO because HTML tags and content play a crucial role in improving SEO.
- When new data is added, our JavaScript file and bundle will grow, which can slow down our website speed.
- Security issues such as exposing secret APIs, keys, passwords, and sensitive information are not recommended in client-side rendering (CSR) as it is generally less secure. There are increased chances of hacking due to the visibility of sensitive data in client-side code.

## Server side Rendering:

Server-side rendering involves loading data on the server and rendering the entire application in the browser by generating HTML in response to requests made from the browser.

<img src="image-2.png" width="300" height="200">

### Advantages of SSR

The benefits of server-side rendering include:

#### 1. Improved Initial Page Load Time:

Server-side rendering reduces the initial page load time by generating HTML on the server and sending it to the client, allowing users to see content more quickly.

#### 2. Enhanced SEO:

Server-side rendering improves search engine optimization (SEO) by ensuring that search engine crawlers can easily index the content of web pages, leading to better visibility in search results.

#### 3. Better Performance on Low-powered Devices:

Since server-side rendering generates HTML on the server, it reduces the amount of processing required on the client-side, resulting in better performance on low-powered devices or slower internet connections.

#### 4. Support for Social Media Sharing:

With server-side rendering, web pages can be fully rendered on the server before being shared on social media platforms, ensuring that shared links display correctly and contain relevant content.

#### 5. Progressive Enhancement:

Server-side rendering allows for progressive enhancement by ensuring that the core content of the web page is accessible even if JavaScript is disabled or not supported in the browser.

#### 6. Easier Debugging and Testing:

Server-side rendering simplifies debugging and testing processes since rendering occurs on the server, making it easier to identify and fix issues related to page rendering and content delivery.

---
# Hydration :

