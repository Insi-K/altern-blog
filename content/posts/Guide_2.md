---
title: '2D Game Graphics Setup (C++ Method - Advanced)'
date: 2024-01-15
author: "Guide" #Using author as category display instead
url: "/post_2024-01-15/"
draft: true
---
One of the issues of using Unreal Engine for 2D game development is the struggle to get sprites placed in the world to look exactly as their source assets. Contrary to other engines such as Unity or Game Maker, Unreal Engine enables by default a post-processing effect that alters the looks of any 2D texture placed into a 3D environment (i.e: sprites tend to look more saturated and slightly blurrier). This is more noticeable when using "pixel-art" assets.

Despite the fact that this is a common issue encountered when starting a project from scratch, I haven't came across many forums that covers this topic and the closer I got to solve this was to "modify" how postprocess affects the final render. It turns out there is a way to get rid of this "postprocess effect" that is being applied on the camera during gameplay, which I had accidentally discovered browsing on the web. Credits to Rocky Mullet for coming up with this approach.

IMPORTANT: For this method, it is necessary to enable C++ scripts in your UE project. Nevertheless, this tutorial wont cover C++ in detail, so anyone with no background in coding should be able to get this done.

1. Enabling C++ in your project
2. Creating the Game Mode script
3. Setting the game mode in your level