# Development experience of an Atri App creator

1. The framework is evoked through the `Terminal` from inside the project repository.
2. The software runs locally on the user's system during the development period. 
3. The user events are compiled at each `Build and Run`. This generates the corresponding code and automatically saves it in the project repository.

> 💻 **Code is always available to the user**

4. Besides, Atri developers do not need to write REST APIs.  Instead, they rely upon the Atri object model which acts as a single source of truth. 
   - Frontend and backend teams now do not need to spend time in maintaining documentation for their APIs 
   - This also has other benefits such as reducing compliance breaches because it is not possible to accidentally send sensitive information from backend to frontend without modifying the object model. 

> 🤯 **No REST APIs**

#### Contextualizing development experience 

To contextualize this development experience, we can think of how web developers build a React app using the `create-react-app` library. 
- The library abstracts away many of the commonly required, cumbersome tasks (both easy and hard problems).
- At the same time, developers still retain complete access and control of their code. 
