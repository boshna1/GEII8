Game Engines Implementation Lecture 8

Road Fighter

Observer

For the observer pattern, I made an interface with FuelUp and SlowDown Functions to be used in the player, the listener and have the fuel cars and normal cars be the notifiers. The way I have it is when the player collides with a fuel car, it calls FuelUp, when it hits a normal car, it calls SlowDown. The SlowDown Interface sets state to slow down and fuel up increases fuel by 500.

State

For State pattern I made enumerator states for being normal, being slowed, and no fuel. Normal is normal speed, slowed is reduced normal speed, and no fuel can't move. SetState function would be called in the player with the inputted parameter and set certain speeds for each one.

Fuel Cars are green
Slow Cars are red
and the end line prints a Finish! string


For the Dirty Flag pattern

I used a UI element that would appear when finishing the game/reaching the end point. It is by default marked as not dirty, but when the car collides it marks the variable as true on the UI and calls the function to activate it. Checking if dirty and if so reveals the text. What I'd do differently is have variables that don't need constant updates in my version of the game in which I am building, and make it fit more around to what I need.

For the Object pooling pattern

I had a lot of logical trouble because when I initially made the Road Fight project, I didn't make the different car types inherit a more abstract version, so everytime I had to assign it to an array or call a variable/function I had to make 2 paths differentiating which one it is. I have logic in which I think is supposed to work, and is of object pooling, but is non-functional because of my previous setup. What I'd do differently is apply previous design patterns, even when not explicitly needed so that it saves time and future error.

What I learned is that these patterns are relatively easy, it is just the setup and way I build things in the level makes it difficult. Applying previously learned patterns would help in this both in logic and time. What I also learned is try not to make things too complex as it could eat up a lot of time, but still emulate the pattern desired in a creative way, rather than, again, complex. Logic is present in the blueprints, but functionality is limited unfortunately.
