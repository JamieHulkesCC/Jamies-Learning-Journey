# Jamies-Learning-Journey
Programming learning journal

## 28/09/2021
Started Year 2 Semester 1 programming course

## 02/10/2021
I found a YouTube video by Brackeys (which is a very reputable channel which is focused directly on the unity engine). This video explains how to make a working save and load in a game which is something that I have never been able to impliment into my games,as I have never had the time learn how to intergrate the system with my code. So I want to use this video because it with give me the fundementals to this system and hopefully allow me to understand it enough to be concious of implimenting it when I start my next project so it will be easy to add.
https://www.youtube.com/watch?v=XOjd_qU2Ido&list=RDCMUCYbK_tjZ2OrIZFBvU6CCMiA&index=2

## 05/10/2021
I started working through the tutorial in class, however I did a minor set back where Brackeys was using a premade scene for the 'fake game' that this system would be applied to. So, to resolve this a I made a similar project myself which was relatively basic where it just allowed to to change the value of the data of both the 'level' and 'health' so that I had some data that I could save and then load. This tutorial continued to explain that this is one of the best save systems that you can get in Unity because it saves the files as binary. This is really import because it basically encrypts the values so they are really hard to alter which is essential considering the majority of the time the values that these files will be holding would durastically be able to manipulate game progess which as developers we want to restrict as much as possible.

I managed to get the complete tutorial finished within the lesson however I will have to go back through some of the parts where he goes over how the system works as some of it is quite hard to get a complete understanfing of straight away so hopefully knowing the theory behind the system as well as having this pracctical example that I have made will help me be able to explain the process in the format of a tutorial to gain a complete understanding for myself and be able to use it easily for my AGP.

## 12/10/21
I once again did some searching online for my next tutorial project. I wanted to work on some menu systems as I feel that they are what I am weaker at within unity as I don't have much experiance with them specific systems whereas I am quite confident with most of the other important aspects of the engine. I found this urge to want to make menus while I made the save system as that gave me some inspiration. After searching on YouTube I found this tutorial: https://www.youtube.com/watch?v=3_xHu-JCkl4

This tutorial was a selection menu where you can allow the player to choose who they play as before the game begins. The tutorial that I selected to use for this project also had some nice juice options to add at the end of it so I could also get some extra experiance with that side of game development after building the core system. The tutorial started with a base scene straight away which was the first issue that I faced as I was aiming to complete this tutorial solely individually whereas the person instuction the video assumed that people partaking in the tutorial already have a game they can impliment this system to. So, at first I thought that I would have to make up a fake game scene to mimic the example that they had already constructed but then I realised that he had a link to his github where you could download his project files if you didn't already have a game to impliment this into.

## 19/10/21
In the recommended videos section of the previous tutorial that I worked on there was another interesting tutorial which would help with my juicing process on the menu system that I had started to gain an understanding for at the end of the last tutorial. The video shows you how to impliment really nice scene transitions using some simple code and then Unity's animation components. Whats also really nice about this video is that once you gain an understanding, it's a very simple process to adapt the result to make your own transitions more unique and better suited to whatever project you are working on. Here is a link to the tutorial that I followed https://www.youtube.com/watch?v=CE9VOZivb3I&t=864s. 

I made a few novice mistakes that I should know better than when first working with the multiple scenes. The first was forgetting to reference Unity's Scene Management within the script and the other was simpily forgetting to add the scenes that I wanted the transition to occur between to the build of the game itself in the build settings. Obviously they were simple mistakes which where fixed very quickly. After this tutorial, I realised that the main focus was on the animation element and not on the code which meant that it wasn't the most optimal. It changed scene on a mouseclick by using a void that would activate on that action and then the code called out for the next scene which is fine unless there are menu buttons where you need it to be more specific so I created a string which isn't ideal but for scene transitions I think I could make an exemption as theres not much better alturnatives and most games arent scene heavy so there shouldn't be any overwhelming errors if there are any at all.

## 26/10/21
As an artist I wanted to get into the side of Unity that was considered its own form of art - technical art. This is of course shader code, but as I was still trying to learn a lot of the core systems of Unity, I decided to learn the shader graph as nodeing is something that I am more familiar with. This is because I use a program called Substance Designer when I am creating art to make procedual textures for my models. The software just like Unity's shader graph uses nodes to create texture maps to the channels that a material needs to work hand in hand for every aspect of the material to work properly. The difference is that Unity's textures created this way are rendered in real time as they can update to animate and also have the capability to effect objects based on their movement and similar factors. So, I then looked on YouTube for another tutorial which I felt was relevant. This tutorial was a shader for potion bottles and more specifically the shader worked on the fluid within the bottle and how it moves and wobbles when the potion bottle is moved about. I thought this was relevant because I want to model more characters and having a potion bottle buckled to their belt or something similar would make the whole piece much more impressive. I also thought that this was a nice and simple shader to learn with as I had a lot of knowlege already but just in a different application. The link to the tutorial that I followed is here: https://www.youtube.com/watch?v=tI3USKIbnh0

Working through the tutorial, as I expected it was some what familiar to me aside from the different names the nodes had and slightly different controls. I found that the shader graph was more interesting because open properties could be edited in the inspector and everything working in real time made results very fun to play with and experiment. One of the first issues that I delt with was the clipping of the liqid with the glass. On the outside it didn't get affected but on the inside you could see that the top of the water was actually infact the backfaces being rendered in a different colour because of the clipping it caused for the edges to be defined which meant that it wasnt flat shaded making it look like one face on top like it should've. The fix for this was quite simple, all I had to do was just scale the water to be smaller ever so slightly and it looked perfect after that. The tutorial also didn't really hold your hand by pursuing a step by step formatt which I much prefer because it prevents me from brainlessly following along and not learning, which really helped me understand the exact process as I had to keep pausing and looking up what nodes did what they were showing on the screen. By breaking this down and doing this research I grasped what each node did in order to manipulate the material to get the result that I wanted. This will help in the future because I will know exactly how these nodes will affect the shader that I am working on.

## 09/11/21
It was now time to move onto the next section of the module which was making a package with a few components that could be reused for a game that I may want to develop in the future. I still felt like I had a big gap in my Unity experiance with UI so I wanted this game to be UI based. I have always loved a game of Jackbox during breaks of working on games with the people that I have been developing with so I decided to make a quiz game package which had all the core components. I also planned to make all of the components completely customizable within the Unity inspector, so when a user downloads my package they can make a completely new game without having to touch any of the code. This makes the process of using my package non-destructive as code is not being changed just data inputed to each of these components. The way I started was by looking at a tutorial I could work from to get an idea of how to make a quiz games core and then I would edit it to make it my own and also layer more components on top of it to make it more fleshed out and helpful to users who are looking to make their games made with this package stand out. The YouTube video that I watched to get the core ideas from was: https://www.youtube.com/watch?v=G9QDFB2RQGA

So the main part of the tutorial I wanted to take some direction from was the quiz manager component as it used a nice and optimized code base to get a nice editable inspector from. The main issue that I found was with the array where it took me a couple of attempts to get right because I kept getting red compiling errors which said that I had gone out of the array. I think this is because I forgot that arrays start at zero which means the length of them is minus one to the length of what the array is. On top of this I also came across some errors when I tried doing script communication because I was unaware how it worked. The main quiz manager communicates with other scripts and by following the code in the tutorial it worked but as I want to edit this code to customize this package down the line I needed to know how it worked properly. So George expalined to me how I could get scripts to communicate in my future projects.

## 16/11/21
I was now just finshing off the coding of the quiz manager and finishing off with some of them bugs that I came across. I found that a few of these bugs that came from the array probably occured because I didn't have much data that I gave the script so how could it possibly work like a full component without some example data. So I decided to make some example quiz questions and answers in order to test if the manager was actually working properly and weather I would still run into these red compling errors. After adding three examples of a question and answering system I playtested the game a bunch in many different combinations to see if glitches were occuring in any way the game was being played and the red compling errors did not show again. So luckily that error was fixed.

So there was a score system incorperated to this quiz manager where everytime you got a question right it would give you a point but 

