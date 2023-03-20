## 1. LifeCycle
1. lazy loading -- Tomcat only loads the servlets that are required to serve the initial request, and defers loading of the other servlets until they are needed, the execution order is constructor() -> init() -> service().  
2. service() -- service is called by every request.  
3. destroy() -- destroy() is called When stop the web application.  

## 2. Servlet request dispatch
service() handles all requests.  

## 3. Servlet Hierarchy
![image](https://user-images.githubusercontent.com/43444919/226262609-df5c213e-1e29-41b8-983b-84509be99be0.png)

## 4. ServletConfig
### Both Servlet and ServletConfig are created by tomcat, and used by web project, each Servlet has its own ServletConfig.
1. getServletName() -- get name of the servlet.  
2. getInitParameter() -- get <init-param> which configured in web.xml.  
3. getServletContext() -- get ServiceContext object.  
  
## 5. ServletContext
### Intro
1. ServletContext is an interface to define servlet's context.  
2. a web project has only one ServletContext which represents the entire web application.   
### Usage
1. retrieve <context-params> that configured in web.xml
2. retrive projectPath, getContextPath(), getRealPath()
3. provides a centralized location for storing and accessing application-wide resources, getAttribute(), setAttribute()



