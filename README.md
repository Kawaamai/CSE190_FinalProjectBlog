# CSE190_FinalProjectBlog: (Astroid) Space Pong

## Table of Contents

1. [Blog 1](#blog-1)

<a name="blog-1"/>
## Blog 1

Project Name: (Astroid) Space Pong (astroid part TBD)
Team Members: Alan Mai

### Project Description

2 Players at either end of a tall long box play ping pong with a large, slow moving ball. On each end of the box, there is a grid of hand holds (spheres or cubes) that each player will use to move up and down, side to side on their end of the box. The players can ~~hit the ball with their hands (or some modeled racket)~~ force push the balls with their hands, until it passes the grid and hits a player's wall, resulting in a point for the other player.

If able to, floating cube "astroids" will be spawned in the play area, that can interact with the ball.

```
       grid offset from walls to allow space to climb around
   v----------------v
|----------------------|
|  .                .  |
|  .                .  |
|  .                .  |
|  .                .  |
|  .                .  |
|  .                .  |
|----------------------|
```

### Technical Details

- UDP server using `yojimbo`.
- PhysX physics engine for physics simulation, simulated on both server and client, with server handling corrective updates.
- ~~Rackets~~ Play ball and/or play area modeled in Blender.
- Audio through `OpenAl` as background music, or a fanfare when a player scores.

### Progress Screenshots

UDP server and client transmitting sample transform data.
![UDP Server and Client](docs/CSE190FinalProjectBlog1_udpServerExample.PNG)

Example scene with physics and force push on trigger pull.
![physics example scene force](docs/CSE190FinalProjectBlog1_physicsexample.PNG)

