---
type: ProjectLayout
title: The HUD - It's Only Money
date: '2024-12-12'
client: Usual Suspects
description: >-
  An overview of the HUD and some insight on the creative and functional
  decisions taken with the layout and elements inside.
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
I wanted to go for a more skeuomorphic design with the HUD for It's Only Money. Being part of a small team and having full control and creative freedom with the UI meant I could go for something less by the books and a bit out of my comfort zone. What I found was that I really enjoyed the ability to add lots of extra details that I might not have with a cleaner more minimalist design.

![](/images/MoneyTicker.jpg)

The first thing I got my hands on when starting on It's Only Money was the Money Ticker - an important part of the HUD as making money is the main goal of the game and it needed to feel satisfying to make and spend money. Five pieces of information get shown here, the current amount of cash in the player's wallet, their wallet limit, their bank card amount and limit, and the delta amount of cash coming in or going out of their wallet.

Because this widget gets used in a lot more places than just the HUD I'd set up a couple of different functions for adjusting the current amount of cash being held. One would animate the whole ticker, re-rolling each digit and locking them in individually while spewing out or sucking in the difference. This was treated as more of a spectacle for the player, the animation taking longer with satisfying sounds and cash particles dynamically set to how much money was coming in or going out. The less in-your-face quick option that was used more in shop screens would only roll the handful of digits that needed changing and the limit of how many particles would spawn was significantly less.

This ticker also shows the wallet and bank limits as lerping bars that change colour as they get closer to the limits. When at the wallet limit, the green border would become full and red, a lock would appear over the cash icon and the digits would momentarily disappear to allow "Cash Limit Reached" text to appear. The whole ticker would also shrink and animate away the bank cards when the player wasn't in a shop or when money wasn't being transferred in or out.

![](/images/ItemsIn.jpg)

Items coming in to the player's inventory was also quite important. In this area I put an encumbrance bar that appears for a couple of seconds when over 80% weight capacity, and when the player reaches 95% this bar stays on screen so they're not surprised when they reach the limit or go over.

Above that I show the items they've just received in their inventory (ManageMe app), along with the name and sell price of those items. I also show items they receive for their houses, wardrobe and other unlocks with appropriate labels for which app or area in the game they can access them.

![](/images/BountyTicker.jpg)

In action here is the Bounty Ticker. Crime is a big part of an open-world crime game, go figure, so tracking and showing the player their bounty amount and bounty tier is important. When a crime is committed, the siren lights up top will flash and a popup will show how much the bounty is increased by, what the crime was and who committed it (handy in multiplayer as it's a shared bounty). Below the bounty amount is the current tier, shown by name and also a light bar with four levels. At the bottom are the current cops patrolling the area, when attacked they flash red, when defeated they ghost out and when spotted they get icon added to them.

![](/images/Vitals.jpg)

Vitals! They are vital on a HUD. When not in combat mode the player is shown their Health, Hunger and Stamina. Increasing the hunger bar will give the player a buff to their damage multiplier.

Entering combat mode the vitals area animates and grows to show more information and emphasizes the Health and Stamina dials that become more important when fighting. Now the player can see their Combat Moves they have equipped, their current weapon and its durability along with the amount of damage it will produce. Each part animates as you'd expect, with particles spawned when healing, dials shaking and glowing red when damage is taken or durability is lost and Moves cooling down de-saturate and show the cooldown time with a progress bar and text.

![](/images/PinnedItemsx.jpg)

The pinned items hotbar in the bottom left of the screen works like any other hotbar to select an item to be held and interacted with. It also has a quick select screen that pops up when the player holds the matching slot key/button. This screen lets the player quickly swap out a pinned item to anything else from their ManageMe inventory and has filters that can be turned off or reconfigured in ManageMe to determine what item types autofill that slot in the future.

#### Other parts of the HUD you'll notice in the overview video:

The Inspection Panel when following civilians shows different attributes of that civilian so they can determine if it's worth it to pickpocket or fight them.

The ModShop panel shows on vehicles and informs the player about what mods are installed on a parked vehicle and if they're discovered or not - letting them decide if it's worth stealing and crushing for the undiscovered parts.

The Compass at the top of screen was a later addition that came during Early Access after a lot of requests. The location pins fade in and grow as the players gets closer them. To help with readability I also made them tint a little darker if they were further away as lot of them can overlap. Undiscovered pins show here as well as grey question marks and I found that really useful for players to discover more parts of the city they might have missed.

The EXP bar and popups also came at the end of Early Access. The EXP popup runs on a timer and if more xp is gained while a popup is still visible it will add to it and replay the animation. When EXP is gained the bar in the top right will flash in a similar colour to the icon while it lerps and the bar will expand to alert the player if they have stat upgrade points ready to spend.
