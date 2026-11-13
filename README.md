# OctoAuctionator - Fixed and improved

The classic **Auctionator 2.6.2** auction house addon (Buy / Sell / More... tabs) ported to **OctoWoW 1.18.1** (1.12.1 client).

Fixed and improved. Free and open-source.

<img src="screenshots/octoauctionator-buy.jpg" alt="OctoAuctionator Screenshot Buy" width="600" height="340">

<img src="screenshots/octoauctionator-sell.jpg" alt="OctoAuctionator Screenshot Sell" width="300" height="170"><img src="screenshots/octoauctionator-listings.jpg" alt="OctoAuctionator Screenshot Listings" width="300" height="170">

<img src="screenshots/octoauctionator-options-tooltips.jpg" alt="OctoAuctionator Screenshot Options Listings" width="300" height="293"><img src="screenshots/octoauctionator-fullscan.jpg" alt="OctoAuctionator Screenshot Full Scan" width="300" height="293">


## What it does

- **Buy:** type a name and press Search. Results fill in while the pages are still coming in, so you can already pick
  a row and press Buy (the scan pauses for the purchase and then carries on). Click **Item Price** to flip
  cheapest-first / most-expensive-first. Recent searches and your own shopping lists sit on the left.
- **Sell:** drop an item in the slot and it searches that item, shows the current auctions and recommends a buyout
  just under the cheapest one. Set the stack size and number of stacks, pick 6 / 24 / 72 hours, Create Auction.
- **Listings:** your listed items: what you have on the AH right now (check for undercuts) and everything you posted before.
- **Full Scan:** optional. Scans the whole auction house and stores the lowest prices for the tooltips.
- **Tooltips:** auction price of an item (and the vendor price if you use SellValue), shown with the game's own coins.

**About speed:** 1.12.1 auction house browsing is quite slow, since the client has a 5 second delay requests, so I'd recommend using AuctionQueryThrottle.dll. More info and download here ![AuctionQueryThrottle](https://github.com/brues-code/AuctionQueryThrottle). It is loaded via VanillaFixes by adding it to your dlls.txt.

## Install

1. Download the latest **OctoAuctionator-X.X.X.zip** from Releases or the forum attachment.
2. Extract it into your WoW `Interface/AddOns` folder.
3. Restart WoW and enable **OctoAuctionator** at character selection.

The folder must contain `Interface/AddOns/OctoAuctionator/OctoAuctionator.toc`.
Turn off other auction house addons (aux, other Auctionator versions) to avoid two UIs fighting over the window.
**SellValue** is optional (vendor prices in tooltips).

## Usage

- Open the auction house: the **Buy**, **Sell** and **More...** tabs are next to Browse / Bids / Auctions.
- The **Auctionator** button (top right) opens the options; **Full Scan...** starts a full scan.
- `/atr clear fullscandb` clears the stored scan prices, `/atr clear posthistory` clears your posting history.

## Credits

**Made by John The Baptist.**

Original addon: **Auctionator 2.6.2 by Zirco** (WoWInterface). This version keeps his interface and code and adapts
them to the 1.12 client and this server.

*It's not much, but it's honest work.*
