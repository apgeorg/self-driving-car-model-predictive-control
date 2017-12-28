# Model Predictive Control


## Kinematic Models
Kinematic models are simplifications of dynamic models that ignore tire forces, gravity, and mass. This simplification reduces the accuracy of the models, but it also makes them more tractable. We want to derive a model that captures how the state evolves over time, and how we can provide an input to change it.

### The state variables

The simulator gives us the below state variables of the car and a series of waypoints with respect to the arbitrary global map coordinate system which we can use to fit a polynomial used to estimate the curve of the road ahead. 

px  | The current location of the vehicle in the x-axis of an arbitrary global map coordinate system.

py  | The current location of the vehicle in the y-axis of an arbitrary global map coordinate system.

psi | The current orientation of the vehicle

v | The current velocity of the vehicle
