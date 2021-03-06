
# Slide 1
* Why Angular2?
* Why I'm here?
* What I'll fucus on? Angular/Application Interface
* Forget Angular1 While Learning Angular2

# Slide 2
* Angular2 is Conceptually Simple
* Angular Prerequisites 
* Angular2 is Reactive -- Like a spreadsheet
* Elements of Reactivity
    * Application Data Object Model
    * Component Object Model
    * DOM/Custom Events
* Object Models
    * Application Domain Object Model
    * Component Object Model
    * Document Object Model
    * Change Detection Object Model

# Slide 3
* Application Data Model
* Document Object Model
* Component Object Model

# Slide 4
* Model Change as a result of Events
* Framework Reacts by Creating DOM
* Browser Paints at the End

# Slide 5
* VM Turn

# Slide 6
* ZoneJS





Angular 2 separates:
* updating the application model (component's state), and
* reflecting the state of the model (component) in the view 
into two distinct phases. 

The developer is responsible for updating the application model (component's state).
Angular, by means of change detection, is responsible for reflecting the state of the model(component) in the view.

Angular does it automatically on every VM turn.

Event bindings, which can be added using the () syntax, can be used to capture 
a browser event to execute some function on a component. 
So they trigger the first phase.

Property bindings, which can be added using the [] syntax, 
should be used only for reflecting the state of the model in the view.


Now, imagine an event changing the model. 
Let’s say I watched the talk “Are we there yet”, 
I really liked it, and I decided to give it 9.9.

The code snippet below illustrates one way to do it. 
The handleRate function is called when the user rates a talk. 
The Talk component just delegates to the App object that updates the model.


http://blog.jhades.org/angular-2-application-architecture-building-flux-like-apps-using-redux-and-immutable-js-js/
## Applications have three types of state

When we mention the application state, we need to make a distinction between several types of state:

* Internal Component State: each component of the component tree (like for example a dropdown) 
  is bound to have some internal state, for example a open flag to indicate that the dropdown is opened
* Global UI State: This state defines the way the user configured the UI: 
  which language is active, which charts are visible, etc.
* Application Data State: This state is the data of the application, 
  for example a list of countries passed to a dropdown

Different strategies might be needed for controlling different types of state. Let's see how the Flux Architecture can help with that.
