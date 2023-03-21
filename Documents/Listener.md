### listen for and respond to specific events or changes that occur within a JavaEE application, e.g. session creation and destruction, attribute changes, context changes etc
## 1. ServletContextListener
Listen ServletContext object's creation and destruction, a ServeletContext is created when web app starts and is destroyed when web app stops.  
### how to implement ServletContextListener
1. write a class which implements ServletContextListener.  
2. implements two call back method defined in ServletContextListener.  
3. configure listener in web.xml
