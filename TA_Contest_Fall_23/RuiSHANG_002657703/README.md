## Game Design tutorial


<br><br>

<p align="center">
  <img src='./img/icon.jpg' width=160 >
</p>

<br>

This tutorial aims to demonstrate how to realize character movements in Unity Engine, which is one of most basic functions in any games. In this project, a character from Unity Asset Store is used as an example, and the entire project file can be download from [Google drive](https://drive.google.com/file/d/1YLikoaRcjS-FViOHQH-A6wQJaJki-yGG/view?usp=drive_link). Due to this tutorial is based on a almost completed project Some parts of the tutorial may not be detailed, so if any problems in following up, plz reach out me on Github.

<br>

### Tutorial Video: 
Available at: https://youtu.be/0BNZHSxVg-I

  [![Watch the video!](https://img.youtube.com/vi/0BNZHSxVg-I/0.jpg)](https://www.youtube.com/watch?v=0BNZHSxVg-I)




<br>

### Procedure

The procedure can be divided into three parts

- Animations: Create character related animations based on original resource

- Arnimator: Build Prefab of thhe character, which includes animations 

- Control Scripts: Programming scripts to control the character

  

Details follow the description below:



#### Animations 

Download resource from asset store:

<p align="center">
   <img src='./img/asset.jpg' width=500 align=center>
</p>

1. Get partial original game material in the Unity Asset Store；

2. Cut frames from original sprite images

3. Build animations
<p align="center">
   <img src='./img/anime.jpg' width=500 align=center>
</p>
P.S

In this project, generative AI also used to provide sprites source for making animation, although the output from Midjourney is not perfect and need further edit in Aseprite

<br>

<p align="center">
  <img src='./img/ai.jpg' width=560 align=center>
</p>

<br>



#### Animator

1. Build an `animator` , which links the transaction between animations

<p align="center">
  <img src='./img/animator.jpg' width=560 align=center>
</p>    





2. Set boundary conditions (contains variables)



#### Control Scripts

Load  `run` variable  from `animator`  and idle from `Sprite Renderer`

1. Link the Character object with a control script

<p align="center">
  <img src='./img/prefabs.jpg' width=360 align=center>
</p>   





2. horizontal moments: Using default `GetAxis` function in Unity engine

3. horizontal moments:  `Input.GetKey(KeyCode.W)`  function and set position transform 

   

<p align="center">
  <img src='./img/playermove.jpg' width=560 align=center>
</p>  




Please view the Game tutorial for details
