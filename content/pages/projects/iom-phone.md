---
type: ProjectLayout
title: Phone System - It's Only Money
date: '2024-12-15'
client: Usual Suspects
description: >-
  The Phone hosts a lot of "Apps" for the player to manage their inventory and
  character, track quests and start mini-games, interact with the map, play
  multiplayer, track accolades and more.
addTitleSuffix: true
colors: colors-b
media:
  type: VideoBlock
  title: Phone System
  url: 'https://youtu.be/WOB06We0CEg'
  elementId: ''
  autoplay: false
  loop: false
  muted: false
  controls: true
  aspectRatio: '16:9'
---
The phone is really just a wrapper that makes some sort of sense lore-wise, an easy way to feed more features to the player without them being able to access them just magically. It also let me just pick a consistent sort of app design theme to roll with for all of the different screens we needed.

IMAGE OF MANAGEME

ManageMe started off as an inventory management screen with extra info about the players vitals, a way for them to customise their combat moves and checked their money limits. From here they can also manage how their hotbar works by choosing what item types each slot should auto-fill with, and they can use or drop any items from their inventory. In the other two tabs there are stat upgrades, mostly work taken from the Metro Dungeon and also DNA Modifiers that unlock when collecting DNA from minibosses around the city. 

IMAGE OF DESTINATION

The Destination app got a huge redesign during Early Access. It used to be quite hard to navigate as the camera was always angled isometrically instead of birdseye view and it wouldn't zoom out far enough. The list of destinations also grew quite large as time went on so creating categories was a must and making the icons for each location type colourful helped distinguish them from each other. Making the compass in the top right rotate accordingly with the current direction and view (if they zoomed in to isometric view it rotates another 45 degrees) also helped a lot with sense of direction. 

IMAGE OF LANDLORD

The LandLord app is where players can look at properties for sale, ones they own, Homies they've freed and their asbestOS inventory of furniture they can place in their houses. 

IAMGE OF WIENER

This is the accolade screen known as Wiener, because one of the main characters is a hotdog man. Players can track the progress of their accolades from this screen and claim the points earned from the ones achieved. Because there are a lot of very similar materials and images being used here I made the silver and gold materials take into account their position onscreen. Things like the white flash travel as a wave from the bottom right to the top left and the overall colour adjusts to be darker if the material is closer to the bottom right of the screen. This helped make the screen not look so repetitive.

I also made the particles that spawn from claimed badges take into account where they're spawning from and how many points they've just earned.
