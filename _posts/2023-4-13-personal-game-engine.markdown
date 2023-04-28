---
layout: post
title:  "Personal Game Engine"
categories: portfolio
---

Here's my personal 3D Game Engine written in C++20. The original intention was to create a game with it, however, this turned into more of a hobby project instead. 
It uses D3D12 as the primary rendering API, with Vulkan as a secondary (unfinished) rendering API layer.

Features include:
* PBR
* Atmospheric scattering (based upon Eric Bruneton's paper)
* Cascaded shadow mapping
* Skinned animation
* FXAA
* Compute particle simulation
* Push-based networking (utilized GameNetworkingSockets)
* Functioning editor (ImGui utilized for the UI)
* PhysX implementation

Pictures:

Atmospheric Scattering
{% include image-gallery.html folder="/projects/engine/atmospheric" %}

Shadows
{% include image-gallery.html folder="/projects/engine/shadows" %}

PBR
{% include image-gallery.html folder="/projects/engine/pbr" %}

Animation

![anim]({{ "assets/projects/engine/anim/anim.gif" | absolute_url }})