---
type: ProjectLayout
title: Metro Dungeon - It's Only Money
date: '2024-12-14'
client: Usual Suspects
description: >-
  A rogue-lite gamemode where I had full creative control over the Game Design,
  Level Design & Lighting, and of course the UI/UX. Completed from start to
  finish with a programmer in 6 weeks.
addTitleSuffix: true
colors: colors-b
media:
  type: VideoBlock
  title: Metro Dungeon
  url: 'https://youtu.be/75_ZNsFZBzM'
  elementId: ''
  autoplay: false
  loop: false
  muted: false
  controls: true
  aspectRatio: '16:9'
---
Creating the Metro Dungeon was an incredibly enjoyable experience and a great opportunity for me to learn new skills. It marked my first time designing a full level in Unreal, writing a comprehensive game design document, and working on the lighting for the level. Additionally, I was responsible for creating the UI for the new game mode, making it a truly hands-on project that allowed me to explore and grow in multiple areas.

![](/images/relics.jpg)

The gameplay concept was relatively simple to develop. We took the already solid combat mechanics from the main game, added more stats, and made it play like a rogue-lite. In the Metro Dungeon mode, players are stripped of all their usual moves and inventory, starting from scratch. At the beginning, they are presented with a choice of three random relics, each made up of a Trigger and an Effect. This system allowed us to create 10 triggers and 10 effects, resulting in 100 unique relic combinations for the player to choose from. The clever part of this approach was that I only needed to design 20 total images and descriptions for the relics, as well as a material to layer the selected trigger and effect images together, simplifying the process while offering variety for the player.

![](/images/fighting.jpg)

The player is chucked into the dungeon to battle enemies and collect crystals, which they can cash in at the end. Surviving each wave allows them to progress, unlocking a series of stat upgrades, combat moves/relics and advancing them through increasingly difficult waves. This creates a challenging loop of combat and progression, where each victory brings more power and more intense battles.

![](/images/stats.jpg)

After defeating each wave of enemies, the player is given a choice of stats to upgrade, with varying levels of potency. These upgrades were primarily based on existing stats, but we also introduced new ones that fit the rogue-lite gameplay, such as thorns and crystal value.

The screen for this was quick to design, as I had already created a bezel and CRT shader for the ATM screen. Using this, I designed a New York Metro-style card payment terminal. With only three options on screen plus a re-roll button, the interface was simple to set up, and implementing controller support was a breeze.

![](/images/timeline.jpg)

Runs in this game mode are dynamic, so the UI for the Timeline had to be flexible as well. Each wave is represented by a red progress bar that fills as enemies are defeated. White dots indicate stat upgrades, yellow icons represent Milestone Relics, and blue icons mark Milestone Moves. The timeline UI was designed to dynamically adjust - whether waves or milestones are added or removed, the interface automatically expands or contracts to accommodate these changes.

![](/images/graff.jpg)

The graffiti was a great addition that really helped make the level feel more unique and immersive. To ensure it performed well, I decided against using decals and instead created a billboard foliage tool. This tool randomized between all the tags, allowing me to place hundreds of graffiti pieces around the map effortlessly. This approach also ensured we were putting a burden on lower-end hardware. 
