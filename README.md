https://sharesub.net - Created by John Bang

Share Sub is a web project of mine using the Express Node.js backend framework. 

The concept is for users to share their subscriptions in an informal way (to show friends which subscriptions they currently have, including Netflix, Spotify, Apple Music, NY Times, etc..)

Please check out and give me feedback ~ :)

It is a dynamically served website that used a Pokedex as a boilerplate.


It contains a lot of useful information related to game data and core mechanics. 

It is not a professional website but it has a beautifully designed user interface powered by Materialize CSS. 

This application is built with Node.js and Express, and it has certain limitations due to the fact that HTML pages are entirely rendered on the server side.

[Pokéapi-v2](https://github.com/PokeAPI/pokedex-promise-v2) is the backbone of the project as it provides all the data used internally inside the routing layer.




### Friend List
* Use the search box on the Pokédex page to look up any pokémon that you are interested in.
* You can search a pokémon by its national pokédex number or name.
* If you do not wish to do manual searching, under the search box, there will be a long list of all pokémon of a particular generation, and you can view their data by simply clicking on the buttons.
* By default, the Pokédex page only shows pokémon in generation one. You can navigate to other generations by clicking on the floating button on the **BOTTOM RIGHT** corner and then click on the generation index number.
* After you selected a pokémon, a new page containing the information about this pokémon will open up.
* The newly opened page will have the pokémon's official artwork, animated 3D game sprites, basic characteristics data, base statistics, and a list of obtainable moves.
* On each individual pokémon page, you can use the **PREV.** and **NEXT** buttons to navigate to the pokémon that appear just before or after the selected pokémon on the national pokédex.

### List of Subs
* The Itemdex page simply lists out most of the items that exist in the official pokémon games with their icon images and brief descriptions.
* Trivial items such as key items are omitted. Items which are no longer available in the newest games are omitted. Items which might be different in different games such as technical machines are also not included.
* Items are separated into categories and sub-categories.
* You can use the floating button on the **BOTTOM RIGHT** corner for quick navigation.

## Issues <img src="https://raw.githubusercontent.com/Kairn/asset-bank/master/pok%C3%A9mon/mini-icons/282.png" alt="icon" height="40" />
* Because of server-side rendering, certain pages (the Itemdex page in particular) that contain lots of fetched data can take more than a few seconds to load before the view is returned. If you are running the application locally and you have suboptimal Internet, the connect could time out on these pages in which case you have to click on the link again to get the page to properly render. Fortunately, Node has internal caching, meaning that once data is received, it stays in memory until you shutdown the server, so even if the server times out while fetching data, the fetched data will no longer need to be retrieved again, and the next request can be processed way faster.


