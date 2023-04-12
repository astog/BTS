# Better Trade Screen

## Introduction
The goal of this mod is to improve the trade screens in Civilization VI and help manage and monitor running trade routes.

## Features
* Shows turns to complete a trade route rather than the distance between the cities.

* Overhauled *Trade Overview* screen.
	* Shows all possible routes, even if the trader is not present in the origin city.
	* Clicking on a route where a free trade unit is not present in the origin city takes you to a free trade unit and opens the *Change City* screen
	* Route entry is colored based on destination player.
	* Player/City header are also colored.
	* Shows origin city and destination city yields in the same screen.
	* Added **Group** and **Filter** settings
	* *My Routes* tab tracks active routes, so you know when a trade route completes.

	![alt text](http://i.imgur.com/3G1PAdh.jpg?1 "Overhauled Trade Overview screen")

* Sort bar in *Make Trade Route* screen and *Trade Overview* screen. Sort the routes by **left clicking** on a button.

	![alt text](http://i.imgur.com/QUTDQYe.jpg "Sort bar - Trade Overview")

* Trade Routes can be sorted based on yields, and turns remaining. Queue multiple sorts by holding **SHIFT** and the left clicking on a sort button. Right click on any sort button to remove it from the sort setting.

	![alt text](http://i.imgur.com/C1T7kPL.jpg?1 "Multiple Sort example")

* When opening *Make Trade Route* screen, the last destination is automatically picked.

* Set a trader to repeat its last route by selecting the **Repeat Route** checkbox when initiating a trade route.

	![alt text](http://i.imgur.com/faLa0b3.jpg "Repeat Route checkbox")

* An additional checkbox is provided that sets the trader to repeat the **top** route from the sort settings when the trade was initiated. This allows the trade route to always be the best one, hence reducing micromanagent of always checking the trade routes.

* Cancel the automated trader from the *My Routes* tab in **Trade Overview** screen.

## Installation
If you are using [Chao's QUI](https://github.com/chaorace/cqui), this mod is already included in it, and requires no extra steps to install. If you are **NOT** using CQUI, follow the steps below:

1. Download the latest release.
2. Extract the downloaded archive to your Mods folder. For me this is in *Documents\My Games\Sid Meier's Civilization VI\Mods*
3. Activate the Mod in *Additional Content* inside Civilization VI.

## Troubleshooting
If you encounter issues with getting the mod working try the following steps:

1. Try installing the Mod into the DLC folder. This folder is the folder where you installed Civilization VI, example *C:\Program Files (x86)\Steam\steamapps\common\Sid Meier's Civilization VI\DLC*
2. Delete the cache. This can be found here - *Documents\My Games\Sid Meier's Civilization VI\Cache*
3. Check out this [thread](https://forums.civfanatics.com/threads/mods-not-working-at-all-help.606288/)
4. If none of the above work, let me know in this repository or [here](https://forums.civfanatics.com/threads/more-lenses.606150/)

## FAQ
**I loaded a save game and the text is all broken?**
> This is a bug from Firaxis. To fix this you have to exit to **destop** and start Civilization VI again.

**I can't see yields for the destination city, where are they?**
>In the previous version, I had a string show that the destination city gains no benefits, but it lead to a lot of cluttering in the screen. Currently, if the destination city has no yield, you won't see any.

**Trade Overview panel does not open in between turns?**
>With v3.0 I blocked the Trade Overview panel from opening since it causes CTD. If you want to unblock this, change the following line in TradeOverview.lua
>
>`local blockPanelInBetweenTurns = true`
>
>to
>
>`local blockPanelInBetweenTurns = false`

## Credits

* @ZhouYzzz for providing the Chinese localization in #161-CQUI
* @deggesim (Simone1974 on Civfanatics) for providing the Italian localization in #250-CQUI
* @e1ectron for providing the Russian localization in #251-CQUI
* @sejbr for providing the Polish localization in #253-CQUI
* @frytom for providing the German localization in #283-CQUI
* @lctrs for providing a partial French localization in #273-CQUI
* @wbqd for providing a Korean translation in #309-CQUI
* @rzucareli for providing a Brazilian-Portuguese localization
