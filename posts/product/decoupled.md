# Can the frontend and backend development be decoupled?

Since Atri framework is a full-stack framework, by definition, it provides the complete ecosystem to build frontend and backend together. However, some web development projects may not need a backend. 

There are two different types of web development projects and Atri framework supports development of both of them. 

1. **Static pages**
   - Static content does not change based on user or her interaction with the content (e.g. "About company" page). 
   - Hence, it does not need a backend.

2. **Dynamic pages**
   - Dynamic content is either personalized for each user (e.g. order history) or dependent on user interaction (e.g. form submission). 
   - In either case, we need to build its backend.

   2.1. **JAMStack**
   - It is a special way of handling backend development work where you outsource almost all of it to services and write minimal backend code.
