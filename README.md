# Toy Room Showdown

A party game for one shared screen and four phones: toy characters escape a room while the other players set off traps against them. Saxion *Project Innovation*, April 2023, 7-person team. I was the sole programmer and a game designer.

<p align="center"><a href="https://youtu.be/fO1U5-CLFus"><img src="https://img.youtube.com/vi/fO1U5-CLFus/maxresdefault.jpg" width="100%" alt="Watch the Toy Room Showdown video"></a><br><sub>▸ <a href="https://youtu.be/fO1U5-CLFus">Watch the video</a></sub></p>

## What I built

- **Networked multiplayer in Photon (PUN)**: four phones join a lobby hosted by the main screen, pick a role and team, and the host loads the game. Movement and rotation sync across screens, and disconnects are handled.
- **Trap system over RPCs**: every trap action syncs between client and server, with per-player cooldowns. The traps are falling block stacks that rebuild, a cash-register drawer, animated fence doors, and trains on a spline track that players can stop and start.
- **Tilt controls**: toys move with the phone's accelerometer, with a speed cap, a filter against shaking, and a boost on cooldown.
- **Phone UI, pressure plates and the final door objective.**
- **Music and sound**: I composed the background music and implemented the sound effects.

I wrote about 4,450 of the roughly 4,800 lines of game scripts.

Scripts: [`PIGame/Assets/Scripts`](PIGame/Assets/Scripts) · Unity 2021.3

`Unity` `C#` `Photon PUN` `Mobile input` `Multiplayer`
