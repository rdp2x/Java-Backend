### External Request Redirection 
- We use `sendRequest()` method for external request redirection. 
- When a redirection from our application to another external application is called **External Request Redirection**. 
- Its a method of `HttpServletResponse` class. 
- `sendRedirect()` method will change the URLs. 

### Internal Request Redirection 
- The **RequestDispatcher** Interface is used to request from another source from same application. 
- No URL is changed in this case. 
- The `forward()` method adds the given content to the pre-existing resource. The browser still interacts with the same page. 

