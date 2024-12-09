# FinalExamRepo
The final exam, recreating Super Mario World

The techniques I have implemented are:
Rim Shader
Scrolling Texture
Hologram
Lambert + Textures Color Correction

Starting with the Hologram for the ghost gameobject:
The hologram effect was used for the eyes and the body of the ghost.
using a diagram I have explained step by step my implementations
![image](https://github.com/user-attachments/assets/d8b2c84d-d033-4a96-9eb3-9bb5bad7e48d)

Rim shader:
I used rim shaders for the coins and to achieve the coin effect similar to the original 2D game but translated into a 3D game environment
This was achieved by using a similar format to the hologram, but without the texture files and instead of doing 1-saturate, I've removed the "1-" in order to let the borders black to achieve a coin effect

Scrolling Texture:
Used a scrolling texture for the background to achieve a sky/cloud moving in the background effect
This was done by using MainTex and ScrollX to only move the texture by the X axis since clouds in a 2D environment only move in 1 direction usually so I made it move from one end to another. ScrollX moves along with _Time which is a default unity component


Lambert Color with Texture:

Added a lambert shader with textures to achieve shadows on all of the envrionment blocks while also being able to customize the color of the texture in order to make the ground, Mario gameobject, and enemies stand out compared to the background sky and blocks
Done by adding the _Color to _MainTex along with using UnityLighting

References used: 

https://www.deviantart.com/thenightcapking/art/Super-Mario-Maker-Grass-Ground-1072347811
https://www.deviantart.com/metagross101/art/Ghost-Texture-380473012
https://dribbble.com/shots/12294406-Super-Mario-Background
https://fastdecals.com/shop/video-game-decals/mario-decals/mario-m-oval-decal-sticker-06.html
