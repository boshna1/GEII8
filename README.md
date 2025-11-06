Game Engines Implementation Lecture 8

Road Fighter

Observer

For the observer pattern, I made an interface with FuelUp and SlowDown Functions to be used in the player, the listener and have the fuel cars and normal cars be the notifiers. The way I have it is when the player collides with a fuel car, it calls FuelUp, when it hits a normal car, it calls SlowDown. The SlowDown Interface sets state to slow down and fuel up increases fuel by 500.

State

For State pattern I made enumerator states for being normal, being slowed, and no fuel. Normal is normal speed, slowed is reduced normal speed, and no fuel can't move. SetState function would be called in the player with the inputted parameter and set certain speeds for each one.

Fuel Cars are green
Slow Cars are red
and the end line prints a Finish! string
