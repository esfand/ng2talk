
Angular 2 separates:
* updating the application model (component's state), and
* reflecting the state of the model in the view 
into two distinct phases. 

The developer is responsible for updating the application model (component's state).
Angular, by means of change detection, is responsible for reflecting the state of the model in the view.

The framework does it automatically on every VM turn.


