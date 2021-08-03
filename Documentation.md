# Documentation
This is the documentation for Marcel Engine.

### Table of Contents  
  * [Getting Started](#getting-started)
  * [The Engine](#the-engine)
  * [Main Engine](#main-engine)
    + [Initialisation](#initialisation)
    + [Rendering](#rendering)
    + [Collision](#collision)
    + [Main Scene](#main-scene)
    + [Camera](#camera)
  * [Objects](#objects)
    + [Creating a new Object](#creating-a-new-object)
    + [Player Object](#player-object)
    + [Text Object](#text-object)
    + [Scene Object](#scene-object)
  * [Graphics](#graphics)
    + [Sprite](#sprite)
    + [SpriteLib](#spritelib)
  * [Sound](#sound)
  * [Networking](#networking)
    + [Server](#server)
    + [Client](#client)
  * [Screen](#screen)
  * [Internals](#internals)
    + [Debug Logger](#debug-logger)
    + [Boot](#boot)






## Getting Started
To get started on a new Game in Marcel Engine please download the latest empty Build from [here](https://github.com/marceldobehere/Marcel-Engine/tree/main/Empty%20Builds).

Then you can unzip the File and Open it in Visual Studio.

Your Code will go into the Your Code.cs file.

There the engine is set up already.








## The Engine
Here are the main parts of the engine

### Main Engine
This is the main part of the engine.

#### Initialisation
You can initialise the engine in two ways:
```csharp
MainEngine engine = new MainEngine((SIZE_X, SIZE_Y, FONT_SIZE), SHOULD_WINDOW_MAXIMISE);
//OR
MainEngine engine = new MainEngine((SIZE_X, SIZE_Y, FONT_SIZE), SHOULD_WINDOW_MAXIMISE, FONT_NAME);
```

#### Rendering
The engine renders a Frame with the RenderFrame() Method.
It takes a number as an input and tries to draw at that framerate. If you use -1 as the input, it will draw as fast as it can.
```csharp
RenderFrame(double prefferedFps);
```

You can also change the backround colour with the SetNewBackroundColour() Method. Its takes an int between 0 and 15 as input.

```csharp
SetNewBackroundColour(int colour);
```

#### Collision
You can check the collision between two objects by using the CheckObjectCollision() Method. It takes two Objects as input and returns true, if they are colliding.
```csharp
CheckObjectCollision(Object a, Object b);
```

#### Main Scene
The engine has an active scene by default.

You can change it with the ChangeActiveScene() command. It takes a scene object as input and replaces the active scene with that one.
```csharp
ChangeActiveScene(Scene new_scene)
```


#### Camera
test


### Objects
This is the Object class. All of the objects in the whole engine and your game will use it.

#### Creating a new Object
test

#### Player Object
test

#### Text Object
test

#### Scene Object
test


### Graphics

The main graphics core.

#### Sprite
test

#### SpriteLib
test


### Sound
Sound manager for the engine.


### Networking
Networking core for the engine.

#### Server
test

#### Client
test


### Screen
Internal stuff ya dont need to care about



### Internals
Internal stuff of the engine.

#### Debug Logger
test

#### Boot
test
