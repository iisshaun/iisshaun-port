---
type: ProjectLayout
title: The HUD - It's Only Money
date: '2024-12-12'
client: Usual Suspects
description: >-
  The HUD for It's Only Money has a ton of unique designs for all of the
  individual elements. Making all of these cohesive with each other was a fun
  challenge.
media:
  type: VideoBlock
  title: HUD Overview
  url: 'https://youtu.be/m4Kj5D99-mw'
  elementId: ''
  autoplay: false
  loop: false
  muted: false
  controls: true
  aspectRatio: '16:9'
addTitleSuffix: true
colors: colors-b
backgroundImage:
  type: BackgroundImage
  backgroundSize: cover
  backgroundPosition: center
  backgroundRepeat: no-repeat
  opacity: 100
bottomSections: []
---
For It's Only Money, I aimed for a more skeuomorphic design with the HUD. Being part of a small team with full control and creative freedom over the UI allowed me to break away from traditional approaches and step out of my comfort zone. What I discovered was how much I enjoyed incorporating extra details - something that might have been lost in a cleaner, more minimalist design. It gave the interface more personality and depth, making it a rewarding creative experience.

![](/images/MoneyTicker.jpg)

When I first started working on It's Only Money, the first thing I tackled was the Money Ticker - an essential part of the HUD, as making and spending money is the core goal of the game. It needed to feel satisfying and impactful. The ticker displays five key pieces of information: the current cash in the player's wallet, their wallet limit, the amount on their bank card, the bank card limit, and the delta amount of cash being added or removed from the wallet.

Since this widget appears in several places beyond just the HUD, I created a few different functions to adjust the cash amount. One animation would play out the entire ticker, re-rolling each digit individually while dynamically adding or subtracting the difference. This version was designed to be a spectacle, with satisfying sound effects and cash particles that varied in intensity based on how much money was moving in or out. The more subtle, quick version used in shop screens would only animate the digits that needed changing, with fewer particles for a less dramatic effect.

The ticker also shows the wallet and bank limits as lerping bars, which change colour as they near their maximum values. When the wallet limit is reached, the green border turns red, a lock appears over the cash icon, and the digits briefly disappear to make way for a "Cash Limit Reached" message. When the player isn't in a shop or money isn’t being transferred, the ticker shrinks, and the bank card details animate away.

![](/images/ItemsIn.jpg)

The process of adding items to the player's inventory was another key aspect I focused on. To help players manage their weight capacity, I added an encumbrance bar that briefly appears when they exceed 80% of their weight limit. When they hit 95%, the bar stays on screen, ensuring they aren’t caught off guard when they reach or exceed the limit.

Above the encumbrance bar, I display the items they've just received in their inventory through the ManageMe app, showing both the item name and its sell price. For items related to their house, wardrobe, or other game unlocks, I include appropriate labels to indicate which app or area the player can access them from. This keeps everything organised and ensures the player knows exactly where to go to use or sell their newly acquired items.

![](/images/BountyTicker.jpg)

Here we have the Bounty Ticker in action. Since crime plays a central role in an open-world crime game, tracking and displaying the player's bounty amount and tier is crucial. When a crime is committed, the siren lights flash at the top, and a popup appears showing the increased bounty, detailing the crime and the player responsible (particularly useful in multiplayer, as the bounty is shared).

Below the bounty amount, the current bounty tier is displayed, both by name and as a light bar with four levels to indicate the heat. At the bottom of the ticker, we show the cops currently patrolling the area. When attacked, they flash red; when defeated, they ghost out; and when spotted, an icon appears above them, keeping the player informed of the status of law enforcement in the area.

![](/images/Vitals.jpg)

Vitals are crucial on a HUD, and in It's Only Money, they play an important role in keeping players informed. When not in combat mode, only the player’s Health, Hunger, and Stamina are displayed. Increasing the hunger bar provides a buff to the player's damage multiplier, adding a strategic element to managing these vitals.

Once the player enters combat mode, the vitals area animates and expands to reveal more information, with a focus on the Health and Stamina dials, which become more important during fights. In this mode, the player can also see their equipped Combat Moves, their current weapon, its durability, and the damage it will deal. Each part is dynamic - particles appear when healing, the dials shake and glow red when damage is taken or durability decreases, and combat moves de-saturate and show cooldown progress with both a visual progress bar and text.

![](/images/PinnedItemsx.jpg)

The pinned items hotbar in the bottom left of the screen functions like any standard hotbar, allowing the player to select an item to hold and interact with. It also features a quick-select screen that appears when the player holds the corresponding slot key or button. This screen enables the player to quickly swap out a pinned item for another from their ManageMe inventory. Additionally, the quick-select screen includes filters that can be toggled on or off, and reconfigured in ManageMe, to control which item types will automatically fill that slot in the future, streamlining the player's inventory management.

#### Other parts of the HUD you'll notice in the overview video:

The Inspection Panel, used when following civilians, displays various attributes of the civilian, allowing players to decide if it's worth pickpocketing or engaging in a fight.

The ModShop panel, shown when interacting with vehicles, provides information on the mods installed on a parked vehicle, including whether they've been discovered. This helps players determine if it's worth stealing the vehicle and crushing it for undiscovered parts.

The Compass, added later in Early Access after numerous requests, features location pins that fade in and grow larger as players get closer to them. To improve readability, the pins darken slightly if they're farther away, helping with readability when overlapping each other. Undiscovered locations are also marked with grey question marks, encouraging players to explore and discover more of the city.

The EXP bar and popups were introduced towards the end of Early Access as well. The EXP popup runs on a timer, adding new XP gains to the existing popup and replaying the animation. When XP is earned, the bar in the top right flashes in the same color as the EXP icon while it smoothly transitions, expanding to alert the player when stat upgrade points are available to be used.
