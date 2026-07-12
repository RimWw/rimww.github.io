---
title: "Pacman Omo"
excerpt: "Made for a Final Project during my 1st year college, a Pacman game with Omori visuals."
header:
  # image: /assets/images/PacmanOmo-cover.png
  teaser: "/assets/images/PacmanOmo-cover.png"
sidebar:
  - title: "Team"
    text: "Solo"
  - title: "Role"
    text: "Programming, Level Design, UI"
  - title: "Development Time"
    text: "2 Weeks"
  - title: "Developed in"
    text: "C Language, Allegro Library"
  - title: "Status"
    text: "College Project, 2022"
classes: "wide"
gallery:
  - url: "/assets/images/PacmanOmo-keybind.JPG"
    image_path: "/assets/images/PacmanOmo-keybind.JPG"
    alt: "Keybind Screenshot"
  - url: "/assets/images/PacmanOmo-leaderboard.JPG"
    image_path: "/assets/images/PacmanOmo-leaderboard.JPG"
    alt: "Leaderboard Screenshot"
  - url: "/assets/images/PacmanOmo-text.JPG"
    image_path: "/assets/images/PacmanOmo-text.JPG"
    alt: "Text Input Screenshot"
order: 6
---

{% include figure image_path="/assets/images/PacmanOmo-cover.png" alt="Pacman Omo Game Screenshot" popup=true%}

> Project Disclaimer: This is a non-commercial, educational project made to demonstrate game programming logic. Visuals shown in these development screenshots utilize assets from OMORI (© OMOCAT, LLC) for educational purpose only. This project is not affiliated with or endorsed by the copyright owners.

This is a game project made for Final Project of "Introduction to Programming" 2022 course during my 1st year in college. This project is written in C with Allegro 5.2 library.

For this project, a basic game template was provided by the course and instructions on how to implement core pacman mechanics were also given. We were tasked with implementing advanced features by ourselves, so I decided to implement various features such as more buffs/game modifiers, custom keybinding, local leaderboard, text input, and save files with my knowledge of C and allegro library at the time.

{% include gallery caption="Custom Keybinding, Leaderboard, and Text Input that I implemented in the game." popup=true%}

We were given freedom to customize our project visuals, so I decided to use Omori assets (for learning purpose) and take one step further by also animating several UI, main menu, and win/lose screen with the available assets. Other than the Omori assets available, I also tried to replicate Omori game's UI using primitive shapes and some text animation.

Looking back, a lot of the programming are somewhat hard coded / brute forced, and the game have several bugs and could still be improved. However, the fact that the game is finished and working is good enough for me, and I'm proud of what I did for my first game ever!
