---
title: "In Desync We Trust"
excerpt: "Made for a Final Project during my 3rd year college, an asymetric coop game about a desynced game world."
header:
  # image: /assets/images/Desync-cover.JPG
  teaser: "/assets/images/Desync-cover.JPG"
sidebar:
  - title: "Team"
    text: "5 People"
  - title: "Role"
    text: "Multiplayer Programming, Project Management, Prototype"
  - title: "Development Time"
    text: "2 Week"
  - title: "Developed in"
    text: "Cocos Creator"
  - title: "Status"
    text: "College Project, 2025"
  - title: "Links"
    nav: game-desync
classes: "wide"
order: 4
---

{% include figure image_path="/assets/images/Desync-cover.JPG" alt="In Desync We Trust Game Screenshot" popup=true%}

> Project Disclaimer: This is a non-commercial, educational project made to demonstrate game programming logic. Visuals shown in these development screenshots may include copyrighted assets used for educational purpose only. This project is not affiliated with or endorsed by the copyright owners.

This is a game project made for Final Project of "Software Studio" 2025 course during my 3rd year in college, made in Cocos Creator. This is an asymmetric coop game, where two players have to communicate and work together to win as each player is playing in a different map/level that is only visible to the other player. I was part of a team of 5 people, and I contributed by proposing the game idea, prototyping, programmed the multiplayer mechanism, and managed the project.

Here's a 3 minute gameplay video of this game: [Gameplay Video](https://www.youtube.com/watch?v=uR00G5HBrnI)

## 1. Game Idea

I thought of game idea after playing several coop matches of [**_Soul Knight_**](https://soulknight.chillyroom.com/et) where often one or more players experience desynchronization in the game, resulting in different objects appearing in each client, or enemies still appearing on one player's screen, leaving them to fight enemies alone while they looked like fighting nothing in other player's perspective.

Inspired by that, and also several asymmetric coop games such as [**_It Takes Two_**](https://store.steampowered.com/app/1426210/It_Takes_Two/) and [**_We Were Here Expeditions: The FriendShip_**](https://store.steampowered.com/app/2296990/We_Were_Here_Expeditions_The_FriendShip/), I devised a game idea about two players escaping from a chaotic desynced world where they must communicate to deduce their true escape path. Each player will have their own corresponding version of the map that is only visible to the other player, forcing players to communicate and direct each other where to go or what to do to reach the goal. Initially, I had some variations idea that follows that general idea, such as puzzles, maze, and even combat, but only a few are later implemented to save time.

## 2. Prototype and Network

As the one that proposed the game idea, I was the one that created a prototype to showcase the idea to my teammates. The prototype is small, only consisting of one level implementing a maze gameplay where each player has their own maze visible only to the other player. Players have to communicate and direct the other player where to go.

This also means that I have to setup and program the multiplayer network in order for the game to work. Building upon the previous homework from the same course where we setup a online realtime lobby room using [_firebase_](https://firebase.google.com/), I expand upon it and customize it to fit my need.

I used [_firebase's_](https://firebase.google.com/) realtime database as the connection point between client, and used room code + password based matchmaking mechanism for players to connect to the same room and start playing together. As the game starts, only minimal data is sent and synced across the database and each client, which is helped by the desynced nature of the game itself.

Later on, the multiplayer programming is handled and improved by me, while other teammates work on the game and level design and other stuff.

## 3. Project Management and Reflection

Initially we were a team of 6 people, but our leader left our group for some unknown reason, and I took the helm as the project leader and manages the project and my teammate to ensure smooth progress and finish the project before deadline. It was rough, as everyone has other exams and projects they have to prepare and finish, our team didn't have the time needed to test and polish the game. But every team member showed up to work together near the end and managed to finish the game before the showcase and presentation time.

While the project wasn't as smooth or as polished as I initially expected, it was another learning opportunity for me, especially about managing scope and expectation with available time and effort, and I'm grateful for it.
