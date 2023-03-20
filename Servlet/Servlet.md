## 1. LifeCycle
### lazy loading 
Tomcat only loads the servlets that are required to serve the initial request, and defers loading of the other servlets until they are needed, the execution order is 
constructor() -> init() -> service().
### service()
service is called by every request.
### destroy()
destroy() is called When stop the web application.

## 2. Servlet request dispatch
service() handles all requests

## 3. Implementing Servlet by inheriting HttpServlet
doGet() for get method and doPost() for post method

## 4. Servlet Hierarchy
![image](https://user-images.githubusercontent.com/43444919/226262609-df5c213e-1e29-41b8-983b-84509be99be0.png)


