## 1. LifeCycle
### lazy loading 
Tomcat only loads the servlets that are required to serve the initial request, and defers loading of the other servlets until they are needed, the execution order is 
constructor() -> init() -> service().
### service()
service is called by every request.
### destroy()
destroy() is called When stop the web application.

## 2. Servlet request dispatch


