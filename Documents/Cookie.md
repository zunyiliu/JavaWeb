## 1. Definition
### A cookie is a piece of data(key-value pair) that is stored on a user's computer by a website. It is sent by a website to a user's browser, and then stored on the user's computer as a file.
1. Client's cookie will be sent to server in every request.  
2. Each cookie has a 4kb max size limit.  

## 2. Create Cookie
![image](https://user-images.githubusercontent.com/43444919/226527590-ab8d2c7f-715c-4178-9ed7-59389f75f6de.png)

## 3. Get Cookies
Cookie[] cookies = req.getCookies() to get cookies from HttpServletRequest

## 4. LifeCycle -- cookie.setMaxAge(time) 
time < 0, delete when browser is closed.  
time == 0, delete immediately after response is received.  
time > 0, delete after age seconds.  

## 5. Cookie Path
### Setting the cookie path is useful for controlling which pages on a website can access a particular cookie
1. cookie.setPath(req.getContextPath() + "/abc") -- requests for /contextPath/abc can access the cookie.  
