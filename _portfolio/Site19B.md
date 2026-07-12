---
title: "Site-19B"
excerpt: "Made for a Final Project during my 3rd year college, a horror adventure game about escaping from a facility where a monster roams around."
header:
  # image: "/assets/images/Site19B-cover.jpg"
  teaser: "/assets/images/Site19B-cover.JPG"
sidebar:
  - title: "Team"
    text: "4 People"
  - title: "Role"
    text: "Game Programming"
  - title: "Development Time"
    text: "2 Week"
  - title: "Developed in"
    text: "Unity"
  - title: "Status"
    text: "College Project, 2024"
  - title: "Links"
    nav: game-site19b
classes: "wide"
order: 3
---

{% include figure image_path="/assets/images/Site19B-cover.JPG" alt="Site-19B Game Poster" popup=true%}

> Project Disclaimer: This is a non-commercial, educational project made to demonstrate game programming logic. Visuals shown in these development screenshots may include copyrighted assets used for educational purpose only. This project is not affiliated with or endorsed by the copyright owners.

This is a game project made for Final Project of "Introduction to Game Programming" 2024 course during my 3rd year in college, made in Unity. It's a horror adventure game about escaping from a facility where a monster roams around. The player must explore and search for items and keys needed to escape, while staying silent and out of the monster's sight. As the game progresses, the player's sanity will also drain, which may cause various effects that make the escape more challenging.

In this project, I contributed in the game programming, mainly working on the enemy AI behaviour, inventory and storage system, interaction mechanic, and more.

Here's a 2 minute gameplay video of the prototype version: [Prototype Video](https://youtu.be/cTPgnyXQ-ow)

Here's a 9 minute gameplay video of the final version: [Gameplay Video](https://www.youtube.com/watch?v=8UdTNxXT12o)

## 1. Enemy AI Behaviour Design

When designing and programming the enemy AI behaviour, I decided to use line of sight and sound mechanic to attract the monster towards the player. When player is within the monster's sight, the monster will pathfind directly towards the player, and when line of sight is broken, the monster will still remember and go towards the last known position of the player. The monster can also hear and pathfind toward sound positions, which are caused by player's activity such as interacting with doors or storage.

When not pathfinding towards the player or any sound, the monster will go into a patrol state guided by a simple navigation system that randomly choose one of the predetermined positions spread across the map weighted by distance to current position in order to make the patrol path feels less random and more deliberate.

## 2. Inventory, Storage, and Interaction Mechanic

The inventory system, storage system, and interaction system are all connected and integral to the game, and I was the one responsible in implementing and refine those system. Initially, the prototype has a basic hotbar system that displayed the items being carried by player, and interactions use items automatically, with a lot of the programming being hard coded or inefficient, making it hard to scale up with more items and functionalities, so I reworked the entire system.

{% include figure image_path="/assets/images/Site19B-protoInv.JPG" caption="Prototype's inventory system" alt="Site19B prototype inventory system" popup=true%}

Just like many aspects of this game, I took [SCP – Containment Breach](https://store.steampowered.com/app/2178380/SCP__Containment_Breach/) as the inspiration and reference on how the inventory should appear and function, and implemented a better system than prototype with more functionality. Now, the inventory has 8 slots, with ability to equip one item, use consumables, and ability to move items to and from storage to inventory with double click. The inventory is now hidden normally and can be viewed by opening up the inventory UI, only showing the equipped item in normal view. Interactions now attempt to use the equipped item if compatible, with a simple dialogue system telling the result of each interactions.

{% include figure image_path="/assets/images/Site19B-finalInv.png" caption="Final version's inventory system" alt="Site19B final inventory system" popup=true%}

While the inventory system itself is quite simple (doesn't support click and drag to move items), it was sufficient for the operations players need to play and finish the game, given the time I had to develop the project.

## 3. Reflection and Others

When we designed the game idea initially, we assumed the implementation was possible using built-in Unity2D features. We encountered some obstacles, such as Unity2D not having proper navmesh feature for 2D, and some problems with how 2D Shadow Caster works. In the end, we found some workarounds, such as using [this 2D Pathfinding package](https://github.com/h8man/navmeshplus) for proper 2D navmesh, and using overlays to hide locked rooms from player's view to fake player's vision restriction.

The game is very far from polished, the map was made too big, the monster moves weirdly, a lack of VFX and SFX polish, and many more unbalanced and untested features leave much to be desired. Yet I'm still proud of the things I did for the project (_especially the whole inventory system_) and learned a lot about gamedev and project management from this project.
