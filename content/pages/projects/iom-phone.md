---
type: ProjectLayout
title: Phone System - It's Only Money
date: '2024-12-15'
client: Usual Suspects
description: >-
  The Phone hosts a slew of "Apps" for the player to manage their inventory and
  character, track quests and start mini-games, interact with the map, track
  accolades and more.
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
The phone serves as a lore-friendly wrapper, providing a seamless way to introduce new features to the player without them feeling out of place. It allowed me to create a consistent app design theme that could be applied across all the different screens we needed. This approach not only kept the UI cohesive but also gave a logical structure to the game's mechanics, making everything feel integrated and purposeful within the game's world.

![](/images/manageme.jpg)

ManageMe originally started as an inventory management screen that provided extra information about the player’s vitals, offered customisation for combat moves, and allowed them to check their money limits. From here, players could also manage their hotbar, choosing which item types each slot should auto-fill with, as well as use or drop items from their inventory.

In the other two tabs, players could access stat upgrades, many of which were derived from the Metro Dungeon mode, and DNA Modifiers, which unlock after collecting DNA from minibosses scattered around the city. This made ManageMe a central hub for not only inventory management but also character progression and customisation.

![](/images/destina.jpg)

The Destination app underwent a major redesign during Early Access to improve navigation. Originally, the camera was locked in an isometric angle, which made it difficult to navigate, especially since it didn’t zoom out far enough. As the list of destinations grew, it became clear that categories were essential to keep things organized. I also made colourful icons for each location type, which helped players quickly distinguish between them.

To further enhance navigation, I added a rotating compass in the top right corner that adjusts based on the player’s current direction and view. When zoomed in to the isometric perspective, the compass rotates an additional 45 degrees, providing a clearer sense of direction.

![](/images/landlord.jpg)

The LandLord app is where players can manage their properties, view ones for sale, and check out the ones they currently own. It also shows the Homies they've freed and keeps track of their asbestOS inventory, which contains furniture they can place in their houses. This app serves as a central hub for home management, offering players a way to personalise their safehouses and interact with various in-game elements related to property ownership and customisation.

![](/images/wiener.jpg)

The accolade screen, known as Wiener (hotdog man, haha), allows players to track their progress on various accolades and claim points for the ones they've achieved. To add visual variety and prevent the screen from feeling repetitive, I used silver and gold materials that adapted to their position on the screen. For example, the white flash effect travels as a wave from the bottom right to the top left, and the colour of the materials adjust to be darker the closer they are to the bottom right.

Additionally, I made the particles that spawn when players claim badges to respond dynamically to their location and the number of points earned.
