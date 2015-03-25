# AeriGUI
AeriGUI is a cross-platform (Windows, Linux & OSX) GUI library written in D using sfml (dsfml).
It doesn't build around OS API's for contol rendering etc. so the rendering is pretty much guaranteed to be the same on all platforms.
It supports advanced GUI rendering with a lot of useful functions to design such as border-styling, image-styling, coloring, positionating in/to contexts.
AeriGUI is suited for regular GUI Application, but also for games and game GUI's, since it's super fast at rendering / drawing; and builds on top of sfml which is meant to be used for games.
AeriGUI has a limited choice of controls, but will of course be updated with new controls over time; however it's super easy to implement a custom control. Take a look at context.d (perhaps contextcontainer.d) and any modules in the controls folder.

### So why AeriGUI and why a new GUI library?
I feel like a lot of GUI libraries tend to complicate stuff for rendering, customization and to make things look good; creating a huge cluster just for the GUI and then all the functions for the application comes.
Besides most GUI libraries are build upon the various OS API's for control rendering etc. which usually isn't the fastest (Ex. GDI) and they aren't that well suited to go with game development, because the painting and events usually can't be associated along with the game libraries.
Ex. you can't mix up GDI with sfml very well.
AeriGUI fixes that problem by using the event calls in sfml for eventhandling and painting, thus making it possible to not even using sfml directly for writing a game.

### More Information
AeriGUI is in no way associated with the D wrapper for sfml (dsfml) or the original sfml project. AeriGUI is a standalone library using sfml (dsfml) for events and rendering.

dsfml: https://github.com/Jebbs/DSFML

Please view the Wiki for more informmation.
