## What is DOCTYPE? What is it for and why is it always at the top of the HTML file?  
  
## What are the differences between null and undefined?  
  
## What are the differences between cookies and local storages?  
  
## What is event delegation?  
  
## What are event capturing and event bubbling?  
  
## What do you care about when developing multiple-language web pages?  
  
## What are the HTTP request methods?  
**POST**, **GET**, **PUT**, **PATCH** and **DELETE** are the main methods that correspond to CRUD actions. There's also HEAD, CONNECT, OPTIONS and TRACE.
  
## What happens when you click on a link or type an URL into the address bar?
1. DNS Lookup starts for *www.example.com.* -> check browser cache, OS cache, router cache
2. Query is passed onto the Resolving Name Server (is the ISP?) -> check the ISP cache
3. Query the Root Name servers (.)
4. Query the Top Level Domain (TLD) Name servers (.com)
5. Query the Authoritative Name servers (ANS) (example.com) -> gives browser the IP address (all steps so far get cached)
6. Browser establishes TCP/IP connection with the server -> '3-way handshake'
7. Browser sends HTTP request -> server sends back HTTP response
8. Browser renders new page/content with received resources
  
## What is CORS?
*Cross-origin Resource Sharing* is an HTTP mechanism that allows a server to restrict which URL's are allowed to load its resources.  
When a browser sends a request, it adds an `Origin: foo.com` header to it. If the request is sent to a different URL (a *cross-origin request*), the server will add an `Access-Control-Allow-Origin: bar.com` header to the response, which specifies the allowed origins.  
If the value of the `Origin` and the `Access-Control-Allow-Origin` headers don't match, the browser will block the response data from being loaded at the client. To prevent this error, the server needs to be configured to include the CORS headers and it has to accept the URL's of interest.
