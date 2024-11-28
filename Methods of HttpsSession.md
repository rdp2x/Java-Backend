- `setAttribute(String name, Object value)` – Binds an object to a given name in the session.
- `getAttribute(String name)` – Retrieves the object associated with the specified name from the session.
- `removeAttribute(String name)` – Removes the object associated with the specified name from the session.
- `invalidate()` – Invalidates the session, effectively removing all session attributes and ending the session.
- `getld()` – Returns the unique identifier assigned to the session.
- `isNew()` – Returns a Boolean indicating whether the session is a new session or an existing one.
- `getLastAccessedTime()` – Returns the time, in milliseconds since midnight January 1, 1970 GMT, when the session was last accessed by the client.
- `getMaxInactiveInterval()` – Returns the maximum time interval, in seconds, between client requests before the session is invalidated.
- `setMaxlnactivelnterval(int interval)` – Sets the maximum time interval, in seconds, between client requests before the session is invalidated.

