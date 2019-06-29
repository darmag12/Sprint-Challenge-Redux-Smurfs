1.  Name 3 JavaScript Array/Object Methods that do not produce side-effects? Which method do we use to create a new object while extending the properties of another object?
.map
.filter
.object.assign - we use this method to create a new object and we can also use the spread syntax

1.  Describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

The store is the single source of truth  because this is where te state lives, which is a javascript object. Actions are also objets that have a type and payload. Data is sent through the store as an action and reducers return to the new state based on the action

1.  What is the difference between Application state and Component state? When would be a good time to use one over the other?

Application state holds the data of the appplication and component state handles data that affects the UI. Application state has global information that many components can be concerned with while component state is something that only the immediate component is concerned with. 
A good time to use component state is a menu bar with an "open" or "closed" state.

1.  What is middleware?

Middleware is a function that is called between dispatch and reducers, and can alter actions or perform other functionalities using them.
thunk lets action creators return a function instead of an action to be able to make async calls. 

1.  Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

thunk lets action creators return a function instead of an action to be able to make async calls. 

1.  Which `react-redux` method links up our `components` with our `redux store`?
connect()
