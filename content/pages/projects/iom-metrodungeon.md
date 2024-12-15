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
Creating the Metro Dungeon was a lot of fun for me and something where I was able to learn a lot of new skills. This was the first proper level I'd created in Unreal, the first time actually writting up a game design doc, along with lighting that level and creating the UI for the new game mode.

![](/images/relics.jpg)

The gameplay was fairly straightforward to come up with, take our already good combat in the game, add more stats and make it play like a roguelite. We take the player and strip them of all of their current moves and inventory from the normal game and start them with nothing. When starting the Metro Dungeon they're given the choice of three random relics to pick from. The relics are made up of a Trigger and an Effect, this let us create say 10 triggers and 10 effects to give the player 100 relics to choose from. Doing this meant I also only needed to make 20 total images and descriptions for all of the relics and a material that would layer the chosen trigger and effect images.

![](/images/fighting.jpg)

The player is chucked into the dungeon to fight and collect crystals for cash at the end. Surviving a wave would progress them through a series of upgrades and more waves.

![](/images/stats.jpg)

After defeating each wave of enemies the player is given a choice of stats to upgrade with varying potency. We were able to base these on mostly existing stats but also new ones that made sense in this gamemode, like thorns and crystal value. The screen for this was also very easy to come up with, having already made a bezel and CRT shader for the ATM screen it was light work to create a New York Metro style card payment terminal and having only three options on screen plus a re-roll button it was very simple to setup controller support as well.

![](/images/timeline.jpg)

Runs in this gamemode can also be dynamic so the UI for the Timeline had to be as well. Each wave is denoted by a red progress bar that fills as each enemy is knocked out, the white dots are the stat upgrades, yellow icons are the Milestone Relics and the blue ones are the Milestone Moves. We can add and remove waves or Milestones and the timeline UI would dynamically grow to accommodate that.

![](/images/graff.jpg)

The graffiti was another fun add and made the whole level feel a lot more bespoke. To make these more performant I opted to not use decals and instead made a billboard foliage tool that would randomise between all of the tags which let me places hundreds of these around the map with ease and not become a burden on lower-end hardware.
