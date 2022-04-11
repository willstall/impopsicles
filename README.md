# **Impopsicles** - *Impossibly Improbable Popsicles*
The combination of crystal-like popsicles and impossible geometry.

[![Movie 01](./videos/01.gif)](./videos/01.mp4)
[![Movie 05](./videos/05.gif)](./videos/05.mp4)
[![Movie 10](./videos/10.gif)](./videos/10.mp4)

***These are rendered in Real-Time via Raymarching in GLSL. Click and Download for Higher Resolution Examples.***

[![Preview 1](./thumbnails/01_thumb.png)](./full/01.png)
[![Preview 2](./thumbnails/02_thumb.png)](./full/02.png)
[![Preview 3](./thumbnails/03_thumb.png)](./full/03.png)
[![Preview 4](./thumbnails/04_thumb.png)](./full/04.png)
[![Preview 5](./thumbnails/05_thumb.png)](./full/05.png)
[![Preview 6](./thumbnails/06_thumb.png)](./full/06.png)
[![Preview 7](./thumbnails/07_thumb.png)](./full/07.png)
[![Preview 8](./thumbnails/08_thumb.png)](./full/08.png)
[![Preview 9](./thumbnails/09_thumb.png)](./full/09.png)
[![Preview 10](./thumbnails/10_thumb.png)](./full/10.png)
[![Preview 11](./thumbnails/11_thumb.png)](./full/11.png)
[![Preview 12](./thumbnails/12_thumb.png)](./full/12.png)

## Idea and Inspiration

## Technology
Impopsicles are first given randomized values in JS. These values are then used to create a custom GLSL fragment shader. The shader is then compiled in real-time. 

## User Input
A collector has the ability to move the Impopsicle around in realtime. While moving, the raymarcher runs is a low-detail view allowing for very quick rendering. When the mouse/touch is released, the piece defaults back into a high-detail mode. The defeault resolution option is 2, but can lowered or raised via 0-9 on keyboard input. 0 being the lowest detail and 9 being the highest. The spacebar can also be used to allow for an ambient rotation action.

## Features and Algorithm

Impopsicles are currently created with a combination or 2 actions. The first action is defining a random popsicle style.

There are quite a few operation styles, each with many characterics.

Styles
  - Vertically Olongated Oval
  - Twist

Style Type
  - Single
  - Double
  - Triple

Style Join Type
  - None
  - Blend

A style is created by picking an itial style w/ a type and join type. Once a style is applied then, each piece recieves a random complexity index. This index represents how many recursive operation sets a piece can make. 

These mutations are combined to form operation sets recursively for extremely interesting results. An operation set can have 1-3 mutations. A duplicative operation is weighted to be done first.

Positional Mutations
  - Rotate ( Single or Multi Axis )
  - Translate ( Single or Multi Axis )

Geometric Mutations
  - Elongate
  - Twist
  - Bend

Duplicative Mutations
  - Reflect
  - Repeat
  - Duplicate ( Single or Multi Axis )

Currently there is a chance between that a piece can recieve between 2 and 5 recursisve operation sets.

Example Operation Sets:
  - Reflect + Rotate
  - Repeat + Twist
  - Reflect + Elongate
  - Reflect + Rotate+Elongate
  - Reflect + Translate

Example of a Seeded Impopsicle:
  - Twist
    - Double
      - Reflect + Rotate + Elongate
      - Repeat + Twist
      - Duplicate + Translate

## Development Status


## About the Artist
