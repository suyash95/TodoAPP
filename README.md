# TodoAPP
    It is very basic TodoApp which is written in javascript. This follows the MVC way of javascript.Let me brief some thing,which has been followed here.

### Model (Data Layer) 

    This is where the data is stored for THE app. The model is decoupled from the views and controllers. Whenever a model changes, it will notify its observers that a change has occurred using an Event Dispatcher.In To Do List App, the Model will hold the list of tasks and be responsible for any actions taken upon each task object.

### View (Presentation Layer)

    This part of App has access to the DOM and is responsible for setting up Event Handlers such as: click, onmouseover, onmouseout, etc. The view is also responsible for the presentation of the HTML. In To Do List App, the view will be responsible for displaying the list of tasks to the user. However, whenever a user enters in a new task through the input field, the view will use an Event Dispatcher to notify the controller, then the controller will update the model.

### Controller (Application Logic)

     The controller is the glue between the model and the view. The controller processes and responds to events set off by either the model or view. It updates the model whenever the user manipulates the view,and can also be used to update the view whenever the model changes. In To Do List app you will be updating the view directly from your model by dispatching an event.
     
### Event Dispatcher 

    The Event Dispatcher is an object that allows you to attach an unlimited number of functions/methods to it. When you finally call the notify method on that Event object, every method you attached to that Event will be ran.
