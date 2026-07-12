---
title: "Block Go Block!"
excerpt: "A short time-loop puzzle game made for GMTK Game Jam 2025."
header:
  # image: "/assets/images/Site19B-cover.jpg"
  teaser: "/assets/images/BlockGMTK-cover2.JPG"
sidebar:
  - title: "Team"
    text: "2 People"
  - title: "Role"
    text: "Game Programming, Level Design, 2D Art"
  - title: "Development Time"
    text: "4 days"
  - title: "Developed in"
    text: "Unity"
  - title: "Status"
    text: "Game Jam, 2025"
  - title: "Links"
    nav: game-block
classes: "wide"
order: 1
---

{% include figure image_path="/assets/images/BlockGMTK-cover2.JPG" alt="Block Go Block! Game Cover" popup=true%}

This is a game project made by me and one of my teammates in [Site-19B project](/portfolio/Site19B/) for [GMTK Game Jam 2025](https://itch.io/jam/gmtk-2025) hosted in [itch.io](https://itch.io/). The theme was "Loop", and we only had 4 days to finish it. This is also my first game jam to participate.

The game we chose to make is a puzzle game where you solve it by working together with... yourselves. Inspired by games with time-loop recording mechanic, such as [Cursor\*10](https://archive.org/details/cursor10_flash), we designed a grid-based puzzle where the player must use time loop mechanic to work together with clones of their past self to get to the goal.

In this project, I contributed in programming all the game logic, designing all three levels, and drawing the character and tilemap sprites. My teammate contributed by designing the UI for main menu, level selection, and during gameplay.

Here's our itch.io page for the game with playable web version: [Block Go Block!](https://rimww.itch.io/block-go-block)

## 1. Programming

The programming for this game is rather simple, validating where the player can go, recording and replaying past players movements, making level components, and making sure that everything works in sync and avoid as many unwanted edge cases as I can. For the players movement recording, I made a simple optimization of storing the number of same consecutive actions instead of just storing actions at each time step, which reduces the amount of data stored (probably negligible...).

There are a few edge cases and bugs that still exist in the game that I know of, but it's pretty rare and with the limited time I have, I moved on to level design. Also, I added score system for points and steps each player took when completing a level, for the more competitive players.

## 2. Level Design

I'm not really a hardcore puzzle gamer or designer, but I had some interesting idea on how to twist this mechanic and force the player to plan their steps carefully, while also keeping it intuitive and not too hard (_hopefully_). I split the game into three levels and one tutorial. For each level, I also added hidden alternative route that will let players to get to the goal with fewer steps/loops. _Who doesn't love finding secrets?_

The first level's idea is simple, introducing the need for player to use their clone to stay on a button to keep the door open for their future selves to get to the goal. Point gems are scattered around intentionally to tempt players to stray from the shortest path to goal, although the clones could also go get those after opening the doors for the future selves, if players want to maximize the points score with fewest steps.

The secret is a button hidden among the walls, which opens a hidden shortcut to the goal. Did I mention that the secrets are only visible when player is very close to it?

{% include figure image_path="/assets/images/BlockGMTK-Lvl-1.png" caption="Block Go Block! Level 1" alt="Level 1 screenshot" popup=true%}

The second level's idea is to add more variations to the doors and buttons mechanic, such as one door requiring multiple buttons being pressed together to open, and that one button can open and close different doors at the same time. So now players can't just mindlessly leave their clones at all buttons. Analyzing where, when, and how long the button should be pressed is the key to solve this level normally.

Or the players can find the secret room, now with its own separate puzzle instead of just a shortcut button!

{% include figure image_path="/assets/images/BlockGMTK-Lvl-2.png" caption="Block Go Block! Level 2" alt="Level 2 screenshot" popup=true%}

The last level builds upon the second level's idea, where now players must handle controlling the doors from two separate area at the same time, requiring more precise timing of when to push and release the buttons to create a smooth passage for the future selves. The secret path is also much harder to find this time, and the player must earn it by exploring and discovering it, which features a hidden maze right inside the walls of the level itself. This level might be a bit too hard, but even I get satisfied after solving this level!

{% include figure image_path="/assets/images/BlockGMTK-Lvl-3.png" caption="Block Go Block! Level 3" alt="Level 3 screenshot" popup=true%}

## 3. Reflection and Others

Given the short time and the knowledge of Unity we had at the time, this project is considered a success, even slightly better than our initial expectation. It's not something innovative or a crazy hit, we had less than 20 browser plays and 13 ratings, but it's in a state that we're satisfied of and people that played it seems to like it.

There are certainly room for improvements, as some ratings pointed out, such as the delay when character moves, ability to view the whole map to plan ahead, and more polish in general. Although I'm probably not going to update this game anymore, those ratings and the overall experience is a great learning experience for us. I even went and tried out many games made by other game jam participants, and amazed of the work that they put out.

Also yes, all the 2D sprites are made by me with [Piskel](https://www.piskelapp.com/), and the itch.io thumbnail and background is made by throwing the assets together in a Unity scene (it gets the job done!).
