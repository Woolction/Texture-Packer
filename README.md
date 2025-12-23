## Texture-Packer

Texture Packer this plugin is designed to consolidate textures into channels of a single texture, like we have RGB channels, and assign each its own map: 

R = Ao 

G = Metallic 

B = Mask 

This allows you to save space in VRam by using one map instead of three separate ones.


The repository contains two main files: 

TexturePacker.cs (an editor script for packing textures), 

ShaderTest (a shader that accepts packed textures). 

First, about the plugin itself; it's located in the Tools folder: It has four slots (you can disable those you don't need), each of which is dedicated to a specific channel and can be selected manually: 

Photo

> **IMPORTANT:**
> If two slots reference the same channel, the information from the latter will be written, as the filling is done linearly. Also, there's no point in changing the slot names; they were created simply for appearance's sake.
