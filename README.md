# 19.-2D-Unity-Game :bird:🏰
While trying to develop a 2D Unity game for a friend of mine (Github: [WolfPark](https://github.com/wolfparktaerim)), I thought that while my friend decides on the art aesthetics of the game, I could further familiarise myself with the process of creating a Unity game by creating a prototype 2D Unity game in advance, with sprites I found from Googling as a placeholder for the art aesthetics. This 2D Unity game can serve as the foundation for any further possible developments in the video game [WolfPark](https://github.com/wolfparktaerim) is trying to develop.

Here is the link of the deployed 2D Unity game on '[itch.io](https://itch.io/)': https://windjammer6.itch.io/2d-unity-game-by-windjammer6 (Click the link to play the game!)

Here is a demonstration of 'winning' the 2D Unity game:


https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/214bc246-3191-4908-95a5-9f5b54e82734



Here is a demonstration of 'losing' the 2D Unity game:


https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/0d0364c2-50fb-4e1c-815c-3e8986bcbbfc



These videos are done by me, using [OBS Studio software](https://obsproject.com/) for screen recording and [VideoPad Video Editor](https://www.nchsoftware.com/videopad/index.html) (by NCH Software) for video editing.

Disclaimer: This 2D Unity game does not work for mobile, only for laptop, PC, or basically any electronic devices that has a keyboard since the game only detects key presses from a keyboard in order to move the character. It does not detect touchscreen controls. (idk how to do that yet, but I believe shouldn't be too difficult) You can open the 2D Unity game on mobile, but you will have no way to move the character.

<br>

**Features of the 2D Unity game:**  
For this prototype 2D Unity game, there is a very vague storyline, as I did not dwell too much on that, but it is more focused towards adding various interesting features via C# programming into the game. Here is a list of features in the 2D Unity game:  
*Character-related:*  
1. Horizontal movement (left and right)
2. Firing projectiles ('bow' and 'arrow')
3. Health system (can take damage from enemy NPCs)

*Friendly NPC-related:*  
1. Interact with NPCs
2. Chief NPC can give the 'bow' weapon to the character

*Enemy NPC-related:*  
1. Chase character when the character enters their trigger range
2. Deal damage to the character when they come into contact with the character
3. Health system (3 lives for small enemies, 5 lives for big enemies) (can take damage from projectiles fired by the character)

*Background-related:*
1. Constructed different sections of the 2D Unity game map, 'Village', 'Open Plains', 'Forest', and the final area with the legendary sword
2. Cloud movement
3. AI generated music on loop, generated by [AIVA](https://www.aiva.ai/)

*Game Objectives-related (in time order of the game):*  
1. Find a way to leave the castle-village (which is that you need to interact with the Chief NPC to get the 'bow' weapon, before the Guard NPC allows you to leave by opening the castle gates)
2. Survive the forest with enemies using the 'bow' weapon (if the character loses all its health then you will lose the game)
3. Obtain the legendary sword at the end of the level to clear the game successfully

Links sources when building the Unity game: https://www.youtube.com/watch?v=XtQMytORBmM&t=1s (Intro to Unity)  
https://www.youtube.com/watch?v=msTvOG4w80I (how to add animation to the sprites in Unity)

https://www.youtube.com/watch?v=CO4BGZOuUkM (how to run C# code in vscode youtube vid)

https://www.youtube.com/watch?v=GhQdlIFylQ8&t=12271s (learn C# code archives youtube vid)

## Table of Contents
Here is a directory of this 'REAME.md' file:
1. [Game Idea](#gameidea)
2. [Building Process of this 2D Unity Game](#buildingprocess)
3. [Deployment Process of this 2D Unity Game](#deploymentprocess)
4. [How to upload a Unity game into Github?](#howtoupload)
5. [How to download and use this Unity source code on Github in your Unity editor/software?](#howtodownloadanduse)

<br>

## 1. Game Idea <a name = "gameidea"></a>  
The design of this 2D Unity game is heavily inspired from [original (OG) Super Mario Bros.](https://supermarioplay.com/) and [Genshin Impact](https://genshin.hoyoverse.com/en), both games that I have played before, with also many aspects of the initial ideas of the game from my friend, [WolfPark](https://github.com/wolfparktaerim). 

*Aspects of the 2D Unity game inspired by the [OG Super Mario Bros.](https://supermarioplay.com/):*  
- The 2D level design
- Character movement
- Enemy NPC behaviour 
- Health system and damage system
- The pixel-style art aesthetics

*Aspects of the 2D Unity game inspired by [Genshin Impact](https://genshin.hoyoverse.com/en):*  
- Friendly NPC interaction feature
- Interaction-related game objective (e.g. the '1. Find a way to leave the castle-village' game objective)

*Aspects of the 2D Unity game inspired by [WolfPark](https://github.com/wolfparktaerim):*  
- The story of the 2D Unity game (though I did not make it as detailed)
- The idea for the respective areas of the 2D Unity game, of a 'home' area, a forest with enemies, and an end objective ([WolfPark](https://github.com/wolfparktaerim) wanted a boss fight, but it took too much effort, so eventually I made the end objective a less programming-intensive one, finding and claiming a 'prize')
- Recommendation of a copyright free, [AIVA](https://www.aiva.ai/) AI music generator, which I used to generate a suitable music for this 2D Unity game

*Source(s):*  
nil

<br>

## 2. Building Process of this 2D Unity Game <a name = "buildingprocess"></a>
This 2D Unity game is built the [Unity](https://unity.com/) game development framework, so obviusly the building process is mainly done in the [Unity](https://unity.com/) editor/software, with C# script components scripting done on the VS code IDE. 

**What are those meta files:**

**About the folders that make up this 2D Unity game:**  
By right, a Unity project/game is actually made up of more folders than those that are present in this repository such as the 'Library' and 'UserSettings' folders, but these remaining folders are ignored by the Github via the Unity '.gitignore' file in this repository (to save space in Github's servers), as they are not as important, and will be re-created anyway when you re-download the source code of this 2D Unity game (basically all the folders in this 2D Unity game repository) and re-import them to the Unity editor/software (more on how to do these in the '5. How to download and use this Unity source code on Github in your Unity editor/software?' section below). 

The 'Packages' and 'ProjectSettings' folders are auto generated folders by Unity as you create a Unity project/game. Not super sure what exactly it is they do, but they are required and are not to be modified to prevent any bugs, together with the most important, 'Assets' folder, that are basically the codes that are essentially your Unity project/game.

The 'Assets' folder is the most important folder that makes up your Unity project/game which, for this 2D Unity game (since the type of folders in this 'Asset' folder varies for each Unity project/game, contains 4 seperate folders, 'C# Scripts', 'Music', 'Scenes' and 'Sprites'.

**'Assets' folder's components of the 2D Unity game and their sources:**  
*C# Scripts:*  
Despite taking the time to learn Unity's C# syntax as documented in my '[16.-Csharp-and-Unity-Learning](https://github.com/WindJammer6/16.-Csharp-and-Unity-Learning)' repository, that is only but a fraction of the Unity C# syntax. 

So most of these C# scripts are actually generated by [ChatGPT](https://chat.openai.com/), while I modified them, based on what I know about the C# programming language and the Unity C# syntax, to fit the requirements of this 2D Unity game.

*Music:*  
Only 1 ambient-themed soundtrack by one of the C# scripts, set on loop, created by [AIVA](https://www.aiva.ai/), AI music generator.

*Scenes:*
"Scenes" folder within the "Assets" directory is a convention that many developers use to organize and manage their game scenes. A Unity scene is a container that holds all of your game objects, assets, and other elements for a specific part or level of your game. The "Scenes" folder is not a special folder in terms of Unity's functionality but is often created by developers to keep their project organized.

Here's how it typically works:

Scene Organization: Developers often create individual scenes for different parts of their game, such as main menus, levels, or specific gameplay sequences. Placing these scenes in a dedicated "Scenes" folder helps to keep them organized.

2D unity game no main menu, only one scene in the game which is the level game scene

*Sprites:*
Bird sprite, which represents the character and NPCs is taken from the 'The Unity Tutorial For Complete Beginners' Youtube tutorial video by Game Maker's Toolkit (link: https://www.youtube.com/watch?v=XtQMytORBmM&t=1s).

The rest of the sprites are taken from Googling. Variations in colour of the sprite, and the 'red bird character sprite with the bow' is done via [Photoshop](https://www.adobe.com/products/photoshop.html), while the scaling was done directly in the Unity editor/software itself.

Text sprites are generated from an [online transparent text generator](https://www.picturetopeople.org/p2p/text_effects_generator.p2p/transparent_text_effect), created by Picture to People. 

Bird sprite taken from the unity tutorial for complete beginners, and the cloud spawner code and idea too


https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/755ab70f-c03e-404d-b0d2-cb05385884ca




https://github.com/WindJammer6/19.-2D-Unity-Game/assets/98175995/ecd2ea31-160f-48bb-b2c9-22edc9b3ba4f



*Source(s):*  
+ https://www.youtube.com/watch?v=GCkq6XqyJZg&t=1529s (Zigurous) (Youtube video labelled 'How to make Super Mario Bros in Unity (Part 1) - Level Design' by Zigurous)
+ https://www.youtube.com/watch?v=SPe1xh4D7Wg&t=3480s (Zigurous) (Youtube video labelled 'How to make Super Mario Bros in Unity (Part 2) - Movement/Physics' by Zigurous)
+ https://www.youtube.com/watch?v=XtQMytORBmM&t=1223s (Game Maker's Toolkit) (Youtube video labelled 'The Unity Tutorial For Complete Beginners' by Game Maker's Toolkit)  this is where i got spawner cloud idea and code ideas from
+ https://www.picturetopeople.org/p2p/text_effects_generator.p2p/transparent_text_effect (Picture to People) (A Transparent Text Generator, to generate the text sprites for this 2D Unity Game)
+ https://www.adobe.com/products/photoshop.html (Photoshop)
+ https://www.youtube.com/watch?v=eB3I4l0AED0&t=81s (Tony Morelli) (Youtube video labelled 'How to play background music in Unity' by Tony Morelli) here is where i learnt to understand the C# script generated by chatgpt to add music to my game and allow it to loop
+ https://www.aiva.ai/ (AIVA)
+ https://chat.openai.com/c/f45522bd-c449-4c7f-aebc-15d58cb1cd44 (CHatGPT) most of the C# scripts components is created first with chatgpt then edited by me to fit my game, and troubleshooting any bugs
 
<br>

## 3. Deployment Process of this 2D Unity Game <a name = "deploymentprocess"></a>

Deployed on '[itch.io](https://itch.io/)', here is my 'itch.io' account https://windjammer6.itch.io/, as recommended by the GDTitans in the youtube vid

Here the specific game link: https://windjammer6.itch.io/2d-unity-game-by-windjammer6

*Source(s):*  
+ https://www.youtube.com/watch?v=UK7SEoiSB2c (GDTitans) (Youtube video labelled 'How To Build & Deploy Your Games With WebGL' by GDTitans)

<br>

## 4. How to upload a Unity game into Github? <a name = "howtoupload"></a>

*Source(s):*  
+ https://www.youtube.com/watch?v=YymhtHtHDb8&t=8s (GDTitans) (Youtube video labelled 'How to Upload your Unity Projects to GitHub In 2023' by GDTitans)

<br>

## 5. How to download and use this Unity source code on Github in your Unity editor/software? <a name = "howtodownloadanduse"></a>

*Source(s):*  
+ https://www.youtube.com/watch?v=I9QK_2QW9W8 (Unity Hero) (Youtube video labelled 'How to import GitHub projects into Unity!' by Unity Hero) 



improvements: boss fight
restart/respawn feature if chafacter dies
area name with trigger and music changes
character is still a bit buggy as it might rotate
friemdly NPCs should not be able to hit by projectiles
enemy NPC should not rotate or leave the ground or chase endlessly? and stop chasing and returning upon character going too far
bug of jumping out of map
safehouse map? To regain HP as safe zone
main menu
replay game or exit upon finishing the game feature
