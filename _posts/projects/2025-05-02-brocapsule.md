---
layout: post
title: "BroCapsule"
author: Zhicheng Zhang
date: 2025-05-02 13:23:43 -0700
tags: [Project]
excerpt_separator: <!--excerpt-->
comments: true
sticky: false
---
BroCapsule is a Unity-based 2D combat puzzle platformer game. It was developed by a six-person team named Team404 as part of the course CSCI 526: Mobile Devices and Game Consoles at the University of Southern California. <!--excerpt-->The development process lasted approximately three months. 

<div style="text-align: center;">
    <p><img src="{{"assets/img/posts/2025-05-02-brocapsule-main-menu.png" | relative_url}}" style="height: 20rem;"></p>
</div>

In BroCapsule, the player must use a spear to overcome various obstacles and reach the destination in each level. When encountering enemies, the player can parry with the spear to disable attacks and gain mana. Mana can also be collected by defeating enemies and picking up spinning collectibles they leave behind. The player can hold a maximum of two mana units. By consuming one mana, the player can throw the spear either vertically or horizontally to attack enemies or create a temporary platform. Additionally, the player can dash and double-jump when needed. To complete each level, players are expected to strategically utilize all these mechanics.

In addition to developing the game, Team404 also created several tools to collect and analyze player data to improve gameplay quality. I was responsible for analyzing the player time-cost heatmap. You can find more details about the tools I developed here: [Heatmap Analyzer](https://github.com/CSCI-526/main-team404/blob/main/Assets/Scripts/Analytics/HeatmapAnalyzer/HeatmapAnalyzer.cs) and [Heatmap Plotter](https://github.com/zhichzhang/heatmap-analyzer-plotter) .