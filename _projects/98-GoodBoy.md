---
title: "Good Boy"
image: "/assets/img/projects/project1.png"
description: "A short puzzle walking-sim developed as a team project for my University's Games and Simulations course."
layout: project
technologies: "Unity, C#"
---
# **Project Details**

- **✅ State:** Concluded  
- **⏳ Duration:** Roughly 2 months  
- **👥 Team Size:** 3 members  
- **💼 My Roles:**  
  -  Gameplay Programmer [Mostly on Level 3]
  -  Game Designer
  -  Animator
- **🛠️ Languages, Engines and Tools Used::** 
    - Unity 
    - C#  
    - Animation Rigging
    - Shaders
- **💡 Key Contributions:**  
  -  Designed and Implemented the core gameplay mechanics for the third Level.    
  -  Developed a PCG algorithm to create the Maze for the third level.  
  -  Developed Portals for seamless transitions between positions.  
  -  Animated the Dog model.

{% include embed/youtube.html id='xzEnkCHLiYU' %}

GitHub: [https://github.com/GamesAndSimulation/ga2024-G1-08/](https://github.com/GamesAndSimulation/ga2024-G1-08/)

# **Introduction**

Good Boy was my final project for the Games and Simulations course in my Computer Science Master's Degree, made by a team of 3 people.

The project had very few restrictions regarding content, giving us creative freedom. However, since it was developed in the context of a Computer Science degree, programming and technological aspects of the game had a heavier influence on our grade. Hence, there wasn't all that much focus in the game's aesthetics, given that we had a very limited time to do so and had to prioritize the programming components of the game.

When brainstorming different ideas, as our team was composed of 3 very close friends, the discussion delve into our personal lives. The three of us had just recently lost our closest pet companions, and it inspired us to honor their memory in the final idea of the game:

```"Good Boy: A puzzle/walking-sim game about a child protagonist that grieves the loss of their dog while dreaming"```

It seemed like a perfect concept for us. The theme was personal, easy to explore, and mixed well with the puzzle genre, which was a great genre to flex our programming muscles, helping us to obtain the best grade we could, whilst creating something a bit more personal.

# **Portals**

🏗️Under Construction🏗️

# **Maze Generation**

Despite most design decisions being done together as a group, the game was divided in three levels, so that it would be easier to divide the work between each one of us, and allow us to express our ideas how we wanted in each of the levels. I was in charge of the third and final level of the game, in which the player must navigate a maze representing of the main character's fear of being lost, through memories that were hijacked by the dog character that arrives to help. This fit the game's context and allowed me to improve my programming skills by creating a maze generation algorithm. All the code for this system can be found on the [GitHub repository](https://github.com/GamesAndSimulation/ga2024-G1-08/tree/main/Assets/Code/Scripts/level3/MazeSystem/).

{%
  include embed/video.html
  src='/assets/vids/good-boy/maze-gen.mp4'
  title='Maze Generation in the Unity Editor'
  autoplay=true
  loop=true
  muted=true
%}

The mazes are generated through a ***Depth First Search(DFS)*** algorithm and are fully customizable through the use of ***Themes***. The bottom-up structure of the system goes as follows:

1. A ***Maze Cell*** is the basic unit of the system. It contains logic for the generation of the DFS algorithm (e.g.: if the cell has visited before, is it part of the solution path, etc.), as well as wall structures and the ***Decorations*** of the ***Maze Theme***.

2. The cells are connected in a grid created by the ***Maze Generator*** game object. This object is responsible for generating the maze through the DFS algorithm, calculate the solution of the maze and apply the ***Theme*** to the ***Maze Cells***, generating the ***Decorations*** in the process.

3. I wanted the several mazes connected, so I created the Multi Maze Generator, which is responsible for generating the pretended number of mazes and connecting them through the previously mentioned [Portals](#portals).

![Desktop View](/assets/img/projects/good-boy/maze-gen-structure.png){: width="1230" height="441" }
_Simplified structure of the maze generation system_


# **Dog Animations**

Given that none of us had experience with 3D modelling, it was obvious to us that we'd have to search the asset store to find a model of a dog to be used in our game. Unfortunately, there were no free-to-use dog assets in the Unity Asset Store that came bundled with animations. Since I had some experience animating with video editing software and even animating rigs in [Garry's Mod](https://steamcommunity.com/sharedfiles/filedetails/?id=104575630), I put myself up to the task of creating all the dog's animations for one of the [free animationless models we found](https://assetstore.unity.com/packages/3d/characters/animals/animals-free-animated-low-poly-3d-models-260727) (**NOTE**: the asset has since then been updated to include a few animations).

I created two animations for walking and running, using a [reference by Stephen Cunnane](https://youtu.be/grGYAnFae7c), and then I also made animations for tail-wagging and barking, without reference. As I became more comfortable with Unity's animation tools and nomenclature, I learned about **animation blending**, and used it for smoother transitions between animations, as well as creating a dynamic animation for the dog's gaze, allowing it to look at game objects, even while moving. Additionally, one of my colleagues created a sniffing animation they needed for the first level and the laying down animation used in the final scene of the third level.

{%
  include embed/video.html
  src='/assets/vids/good-boy/walk-anim.mp4'
  title='Walking Animation'
  autoplay=true
  loop=true
  muted=true
%}

Although the animations look amateurish, I was happy with the result, especially taking into consideration my lack of experience and the limited development time. They portrayed the actions well enough to be easily understood, which was the main objective, and also helped the dog character to become a lot more alive through the dynamic gaze animations.

{%
  include embed/video.html
  src='/assets/vids/good-boy/gaze-anim.mp4'
  title='Dynamic gaze animation'
  autoplay=true
  loop=true
  muted=true
%}

# **Disclaimer**
This game was created for educational purposes, and it is not for commercial use. Given this, the music and some of the models used in this game were heavily inspired/taken from other games, as we didn't have time nor the skill to make our own. All rights belong to their respective owners.