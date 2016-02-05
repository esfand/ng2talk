
Angular 2 separates:
* updating the application model (component's state), and
* reflecting the state of the model in the view 
into two distinct phases. 

The developer is responsible for updating the application model (component's state).
Angular, by means of change detection, is responsible for reflecting the state of the model in the view.

The framework does it automatically on every VM turn.

Event bindings, which can be added using the () syntax, can be used to capture 
a browser event execute some function on a component. 
 So they trigger the first phase.

Property bindings, which can be added using the [] syntax, 
should be used only for reflecting the state of the model in the view.
