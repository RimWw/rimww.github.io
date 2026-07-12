---
title: "Project TCSF"
excerpt: "A prototype of horde shooter gameplay made in Genshin Impact Miliastra Wonderland."
header:
  # image: "/assets/images/Site19B-cover.jpg"
  teaser: "/assets/images/ProtoTCSF-cover.png"
sidebar:
  - title: "Team"
    text: "Solo"
  - title: "Role"
    text: "Scripting, Game & Level Design"
  - title: "Development Time"
    text: "5 months"
  - title: "Developed in"
    text: "Genshin Impact Miliastra Wonderland"
  - title: "Status"
    text: "Prototype, 2026"
  - title: "Links"
    nav: game-proto-tcsf
gallery:
  - url: "/assets/images/ProtoTCSF-gun-m4.JPG"
    image_path: "/assets/images/ProtoTCSF-gun-m4.JPG"
    alt: "M4 Model Screenshot"
  - url: "/assets/images/ProtoTCSF-gun-m250.JPG"
    image_path: "/assets/images/ProtoTCSF-gun-m250.JPG"
    alt: "M250 Model Screenshot"
  - url: "/assets/images/ProtoTCSF-gun-garand.JPG"
    image_path: "/assets/images/ProtoTCSF-gun-garand.JPG"
    alt: "Garand Model Screenshot"
classes: "wide"
order: 5
---

{% include figure image_path="/assets/images/ProtoTCSF-cover.png" alt="Project TCSF Screenshot" popup=true%}

This is a UGC project prototype made in [Genshin Impact's Miliastra Wonderland](https://genshin.hoyoverse.com/en/news/detail/159060). In this project, I learned to use the available framework of Miliastra and attempted to create a horde shooter gameplay. I stopped working on this project due to scope creep, slow development progress, and outdated framework usage.

Here's a short 2-minute video showcasing the prototype: [Prototype Video](https://youtu.be/aZ9Rgn1vDpI)

After learning about the basics of Genshin's UGC Miliastra framework and publishing my first UGC stage, [There Is No Button](/portfolio/ThereIsNoButton), I set my vision on a horde shooter gameplay, similar to [Left 4 Dead](https://store.steampowered.com/app/500/Left_4_Dead/), [World War Z: Aftermath](https://store.steampowered.com/app/699130/World_War_Z/), and many other zombie shooters that I played. I like shooter games, and zombie games, so I wanted to try recreate one with the available tools and framework in Miliastra.

## 1. What I tried to make

Initially, I planned to make a horde shooter game where players must defend and hold out against hordes of enemies for as long as they can. Picture humans staving off waves of monsters onslaught with the few remaining resources they have, slowly falling back as they lose grounds and resources, all to buy time for reinforcements or for other people to escape. It's actually also similar to a gamemode of [Project Untote](https://www.roblox.com/id/games/93031957335865/Project-Untote) that I played before.

Since I like the gunplay of [Left 4 Dead](https://store.steampowered.com/app/500/Left_4_Dead/) and [World War Z: Aftermath](https://store.steampowered.com/app/699130/World_War_Z/), I tried to design the gun and pickup system similar to them, especially World War Z's since they improve upon Left 4 Dead's design.

Some other game design that I thought of to improve upon the ideas and mechanics of similar games:

- Safe Zone around the defense objective, pushing player to gather and defend instead of spreading out.
- Randomizing routes for each playthrough, with multiple possible areas to play in one map, giving a controlled variety for replayability.
- Variations in monster wave size, length, concentration, enemy types and difficulty, etc. to give a feeling of constantly changing situations.
- More emphasis on resource management and utilization, creating sense of urgency from shrinking resources, pushing player to use the most out of their resources
  While not exactly innovative, these are just ideas I thought could improve on the scenario of surviving against hordes of monsters.

## 2. What I learned in this project

I learned a lot about the Miliastra framework while doing this project, including but not limited to:

- Player skills and animation system
- Projectile mechanics, Hitscan attack implementation, and their limitations
- Client side scripting for skills
- Managing game states, game event propagation and processing, etc.
- Optimizing performance to work within load limit
- Creating Custom Models by combining assets of various shapes and colors
- and much more...

{% include gallery caption='Some of the "custom" models that I made by combining assets together' popup=true%}

Some of the challenges I encountered while working on this project:

- Performance cost of Prefab Instantiation on runtime (pooling is possible but only for specific use cases)
- Performance cost of having too many monsters in scene
- Limitations of projectile hit detection
- Hit registration issues
- Lack of options to customize animations, assets, etc.

Despite the challenges, I worked and tested on workarounds and compromises, however after developing for some time, I came to a realization and decided to stop this project, which I will explain next.

## 3. Why I stopped, and how can I improve

I was working on and off this project while studying for my 4th year in college, and I finally realized that:

1. Scope creep: My scope was too big, maybe too ambitious even. I was thinking too far about things I want to implement, when the base mechanic is still not yet complete.
2. Messy systems: I started with making a system with complex features in mind, when I haven't tested with a simpler system.
3. Slowing learning: Due to focusing on making specific features work, I slowed down on learning new features and functions of the framework that would've been more worthy to learn and implement.
4. Outdated implementation: Many of the workarounds that I initially worked on due to the framework's limits and issues become obsolete as the framework is constantly updated with more features and fixes. Things like client side data, UI, skills, and custom models have received their own features from the framework to better customize to our needs. At this point, updating my implementation to use these new and better features will take as much time as just starting fresh and use these features instead.

With that in mind, I took a hard decision of stopping this project and starting fresh. I even heard that the developers of the framework is working on features that will improve shooter gameplay implementations. So, what I learned from this is that:

1. Start small: Reduce the scope, test and prove that it can work with the core features, then expand upon it once it works.
2. More planning: Planning ahead how the systems should be structured will greatly help in expanding and adding features later on.
3. Make it exist first, polish it later: Focus on making it exist and work, then make it more beautiful and smoother later.

The point is, to make the best out of my time and effort, I should prioritize on making and testing the base work before going further to polish each one, creating good systems that can be expanded upon while staying flexible and choosing what works instead of chasing perfection forever.
