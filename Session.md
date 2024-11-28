- A session is something that created/stores the user’s value that can be access all over the project files, unlike _[[Request Redirection|request]]_ object that is used only between two pages.
- The _request_ object gets deleted once it get received by its destination. 

> [!NOTE] Note
> We can carry all the values from one page to another via variables or other stuffs, but it’ll make the web application slow. So this is not preferred, and here **sessions** comes into play. 

- Values needed all over the application are stored in the session and later send to the page from sessions itself. 

#### Creating a session

- We use _HttpServletRequest_ Interface’s `getSession()` method to create a session object. If the session is created, it gets the session, or else, it creates a new session and then gets it. 
- The class used to store the object is _HttpSession_. 
- The method used to store the session data is `setAttribute('key', value)`. This method stores the values in key-value pairs. 
- The method used to receive the values from session is `getAttributes(key)`.  
- To remove a specific value from the session, we use the `removeAttribute()` method. 

#### Deleting a session

- To delete the whole session, we use `invalidate()` method. 

> [!WARNING] Note
> In the _.jsp_ page, the `getAttribute()` methods should have the object named `session`, else it’ll not work and give error.

- There are many way to delete the Session object, like if the browser is closed or using [[Deployment Descriptor]] file (timeout). 

### Internal Working of Sessions

- When a session object is created for a user, a unique **session-id** is generated and is stored on the server. When the user logs in again the session-id is matched and no new object is created again for that user. 
- The servlet select and fetched the data of that given user through this session-id.
- [ ] Similarly, for different users, different ids are created and utilized to fetch their own data only, to avoid data miss-matched. 


