## 1. Definition
1. Responsible for intercepting requests and responses to a web application.  
2. The filter can be used to modify or augment the request or response, or to perform any other pre-processing or post-processing tasks.  
3. Commonly used for authentication, logging, caching, encryption, and compression etc.  
4. To create a filter in a Java web application, implement the javax.servlet.Filter interface and provide an implementation for the doFilter method.  
The filter can then be registered in the web.xml deployment descriptor file or using annotations in a servlet container or application server.  

## 2. LifeCycle
1. Constructor(), init() -- are executed when web application starts(Filter is created once start).  
2. doFilter() -- triggered when a request is intercepted.  
3. destroy() -- destroyed when web app stops.  

## 3. FilterConfig
When Tomcat creates Filter object, it also creates FilterConfig object which contains filter's configurations.  
1. Get filter's name.  
2. Get filter's init-params.  
3. Get ServeletContext object.  


## 4. FilterChain
When a request is sent to a Java web application, the server creates a chain of filters and passes the request to the first filter in the chain.
The filter then performs its processing and can either pass the request to the next filter in the chain or send a response back to the client.  
The FilterChain interface represents a chain of filters that a request goes through. It provides methods for adding and removing filters, as well as passing the 
request and response objects between filters.  


## 5. Filter url-pattern
1. precise match -- /target, path must match /target
2. wildcard match -- /target/*, match all paths starts with /target
3. suffix match -- *.html, match all html files
