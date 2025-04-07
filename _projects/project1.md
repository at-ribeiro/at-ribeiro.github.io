---
title: "Good Boy"
image: "/assets/img/projects/project1.png"
description: "A short puzzle walking-sim developed as a team project for my University's Games and Simulations course"
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
- **🛠️ Technologies Used:** 
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

# **Introduction**

Good Boy was my final project for the Games and Simulations course in my Computer Science Master's Degree, made by a team of 3 people.

The project had very few restrictions regarding content, giving us creative freedom. However, since it was developed in the context of a Computer Science degree, programming and technological aspects of the game had a heavier influence on our grade. Hence, there wasn't all that much focus in the game's aesthetics, given that we had a very limited time to do so and had to prioritize the programming components of the game.

When brainstorming different ideas, as our team was composed of 3 very close friends, the discussion delve into our personal lives. The three of us had just recently lost our closest pet companions, and it inspired us to honor their memory in the final idea of the game:

```"Good Boy: A puzzle/walking-sim game about a child protagonist that grieves the loss of their dog while dreaming"```

It seemed like a perfect concept for us. The theme was personal, easy to explore, and mixed well with the puzzle genre, which was a great genre to flex our programming muscles, helping us to obtain the best grade we could, whilst creating something a bit more personal.

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
# **Maze Generation**

# **Portals**

# **Disclaimer**
This game was created for educational purposes, and it is not for commercial use. Given this, the music and some of the models used in this game were heavily inspired/taken from other games, as we didn't have time nor the skill to make our own. All rights belong to their respective owners.