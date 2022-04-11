# **Impopsicles** - *Impossibly Improbable Popsicles*
A combination of crystal-like popsicles and impossible geometry.

***All pieces are interactive.***

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
Popsicles are delicous, but Imposicles are impossibly delicious. Inspired by amazing artists like M.C. Escher and Andy Warhol, Impopsicles is a long-form generative series that blends light, math, and dessert to shape gorgeous Interactive Popsicles. Each 'cicle' is a just another lick of creation.

## Technology
Impopsicles are first given randomized seed values in Javascript. These values are then used to create a custom GLSL fragment shader. The shader is then compiled in real-time. Raymarching is used to render the scene. Each piece, at it's core, is a uniquely generated SDF ( signed distance field ) that is then modified in unique and unexpected ways.

## User Input
A collector has the ability to move an Impopsicle around. While moving, the raymarcher runs in low-detail mode allowing for very quick rendering. When static the piece defaults to a high-detail mode. The default resolution option is 2, but can lowered or raised via 0-9 on keyboard input. 0 being the lowest detail and 9 being the highest.

The spacebar can also be used to allow for an ambient rotation action.

![Preview 13](./full/13.png)

## Features and Algorithm

Impopsicles are currently created with a combination or 2 actions. The first action is defining a random 'overall' popsicle style. The second action is apply mutation upon this style.

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

A style is created by picking an itial style combined w/ a type and join type. Once a style is applied then, each piece recieves a random complexity index. This index represents how many recursive 'Operation Sets' a piece can make. Operations Sets are a combined group of mutations that are used recursively in order to manifest extremely interesting results. An operation set can have 1-3 mutations. A duplicative operation is weighted as the highest to go first in a sequence.

Positional Mutations
  - Rotate ( Single or Multi Axis )
  - Translate ( Single or Multi Axis )

Geometric Mutations
  - Elongate
  - Twist
  - Bend
  - Wrap

Duplicative Mutations
  - Reflect
  - Repeat
  - Duplicate ( Single or Multi Axis )

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

***Currently, a piece has an opportunity of 2-5 recursisve operation sets.***

## Development Status
Impopsicle already works and renders beautifuly in realtime. That said, development is still very active. The rendering engine is currently being extended to support more styles and rendering techniques. The base algorithm is also being assessed and modified for scale, orginality, and beauty; daily. Additional colors and materials are also being tested and developed.

***The final implementation will not just have blue cicles.***

## About WillStall
Will has been making generative art since before the ye ol' days of flash; 20ish+ years of silly creation. Now he's a designer/developer/engineer/something working in GLSL making realtime shaders.

He's a big fan of community and has run a coworking space, an award-winning game studio, a black-tie award show for creatives, and an event called dev-night that brought together brilliant people on a weekly basis to create nothing more than scenarios of fun.

He's also been known to laugh, make up words, roller skate, and tell people they're lovely wayyyyy too many times.

Some call him creative, others call him Will


