## 1. Definition 
1. Session is an Interface(HttpSession).  
2. Session is to maintain some data between client and server, is built based on cookie technology. Session data is stored in server-side, however
the sessionId is stored as cookie to identify a unique session for each client, with cookie expire set as "session" (meaning it will be removed once browser is closed).  
3. Ever client has its own session, it's usually to store data after user login.  

## 2. Session LifeCycle
