# HTML & DOM
### What are HTML meta tags?  
HTML meta tags are tags that provide additional information about the web page such as the title, description, author, keywords and encoding information to the browser, search engines and other web services. They're located in the `<head>` tag and they aren't displayed on the page itself.

### What is the DOM?
The Document Object Model is the browser's object representation of the HTML code. It is organized into a tree-like data structure of all the elements that constitute the page in question.

### What is DOCTYPE? What is it for and why is it always at the top of the HTML file?  

<br>
<br>
<br>

# JavaScript
### What are the differences between null and undefined?
While they both indicate a lack of value, `null` does not occur naturally. That is, if a variable has the value `null`, it has been assigned it manually. On the other hand, `undefined` occurs when trying to access a variable that has been declared but hasn't been assigned a value yet.

### What is a callback in JS?  
A callback is a function that is passed as argument to another function. They're used to develop asynchronous code.  
  
### What is event delegation?  
  
### What are event capturing and event bubbling?  

### What are closures and lexical scoping?
A closure is the combination of a function bundled together with references to its surrounding state (the lexical environment). Whenever a function is defined, it "remembers" the surrounding scope (and any variables that were accessible). In nested functions, a closure gives you access to an outer function's scope from an inner function.

### What is JSON and what is it used for?
JavaScript Object Notation is a standard text-based format for representing structured data. It is used for storing data and transmitting data over the web. 

<br>
<br>
<br>

# Web & Tooling
### What do tools like Webpack do?
Bundlers are used to resolve the dependency web of front end asset files and package them together into optimized bundles for the browser. This way, the client needs to make less requests to the server when visiting a page.

### What are some ways to decrease page load time?  
* Optimize media such as images and videos
* Serve from closer to the end-user e.g. CDN, Edge
* Employ caching methods
* Minifying, code-splitting

### What are the differences between cookies and local storages?

### What do you care about when developing multiple-language web pages?  
  
### What are the HTTP request methods?  
**POST**, **GET**, **PUT** (update entire resource), **PATCH** (update parts of a resource) and **DELETE** are the main methods that correspond to CRUD actions. There's also HEAD, CONNECT, OPTIONS and TRACE.

### What are the main characteristics of a RESTful API?
* Stateless
* Resources should be uniquely identifiable through the URL (endpoints)
* HTTP request methods used to access and transform resources

### What happens when you click on a link or type an URL into the address bar?
1. DNS Lookup starts for *www.example.com.* -> check browser cache, OS cache, router cache
2. Query is passed onto the Resolving Name Server (is the ISP?) -> check the ISP cache
3. Query the Root Name servers (.)
4. Query the Top Level Domain (TLD) Name servers (.com)
5. Query the Authoritative Name servers (ANS) (example.com) -> gives browser the IP address (all steps so far get cached)
6. Browser establishes TCP/IP connection with the server -> '3-way handshake'
7. Browser sends HTTP request -> server sends back HTTP response
8. Browser renders new page/content with received resources
  
### What is CORS?
*Cross-origin Resource Sharing* is an HTTP mechanism that allows a server to restrict which URL's are allowed to load its resources.  
When a browser sends a request, it adds an `Origin: foo.com` header to it. If the request is sent to a different URL (a *cross-origin request*), the server will add an `Access-Control-Allow-Origin: bar.com` header to the response, which specifies the allowed origins.  
If the value of the `Origin` and the `Access-Control-Allow-Origin` headers don't match, the browser will block the response data from being loaded at the client. To prevent this error, the server needs to be configured to include the CORS headers and it has to accept the URL's of interest.

<br>
<br>
<br>


  
