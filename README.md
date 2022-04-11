# **Impopsicles** - *Impossibly Improbable Popsicles*
The combination of crystal-like popsicles and impossible geometry.

[![Movie 01](./videos/01.gif)](./videos/01.mp4)
[![Movie 05](./videos/05.gif)](./videos/05.mp4)
[![Movie 10](./videos/10.gif)](./videos/10.mp4)

***These are rendered in Real-Time via Raymarching in GLSL.***
***Click and Download for a Resolution Example.***

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


# NEED TO TALK ABOUT IT BEING IN REALTIME WITH GLSL

## Idea and Inspiration

## Features and Algorithm
Each piece recieves a random complexity index. This index represents how many recursive operation sets a piece can make. 

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
  - Reflect+Rotate
  - Repeat+Twist
  - Reflect+Elongate
  - Reflect+Rotate+Elongate
  - Reflect+Translate


## Technology

## Development Status

## About the Artist
