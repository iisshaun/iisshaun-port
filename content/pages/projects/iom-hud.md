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
featuredImage:
  type: ImageBlock
  url: /images/HUDoverview.jpg
  altText: altText of the image
  caption: Caption of the image
  elementId: ''
bottomSections: []
---
![](/images/MoneyTicker.jpg)

The first thing I got my hands on when starting on It's Only Money was the Money Ticker - an important part of the HUD as making money is the main goal of the game and it needed to feel satisfying to make and spend money. Five pieces of information get shown here, the current amount of cash in the player's wallet, their wallet limit, their bank card amount and limit, and the delta amount of cash coming in or going out of their wallet.

Because this widget gets used in a lot more places than just the HUD I'd set up a couple of different functions for adjusting the current amount of cash being held. One would animate the whole ticker, re-rolling each digit and locking them in individually while spewing out or sucking in the difference. This was treated as more of a spectacle for the player, the animation taking longer with satisfying sounds and cash particles dynamically set to how much money was coming in or going out. The less in-your-face quick option that was used more in shop screens would only roll the handful of digits that needed changing and the limit of how many particles would spawn was significantly less.

This ticker also shows the wallet and bank limits as lerping bars that change colour as they get closer to the limits. When at the wallet limit, the green border would become full and red, a lock would appear over the cash icon and the digits would momentarily disappear to allow "Cash Limit Reached" text to appear. The whole ticker would also shrink and animate away the bank cards when the player wasn't in a shop or when money wasn't being transferred in or out.



![](/images/ItemsIn.jpg)
