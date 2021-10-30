# Industries of the Caribbean

Jump to [Design Notes](#design-notes)

## Gameplay Guide

Industries of the Caribbean models a state-run economy where you own the industries and production chain, in addition to the transport network. The economy is export-driven: unless you export a cargo, you don’t get paid for transporting it.

Your island has fertile soil and rich deposits of oil and nickel, but no processing industries to produce valuable products. Initially, the only profitable cargo is coffee, which requires no processing before it is exported. 

Start by exporting as much coffee as you can until you can afford your first processing industry: the sugar mill. After that, unlock new cargo chains by funding the proper industries, as governed by the cargo flowchart and the Import/Export trade deals. Be careful, though, not to expand into a cargo chain before you have the required cargos — for example, the Nickel chain requires Chemicals, which are obtained by exporting Cigars.

### Recommended World Generation settings

* Climate: Sub-tropical
* Sea level: Medium
* No. of towns: High
* No. of industries: Low
* Desert coverage: 0%

### Recommended Settings

* News/Advisors: Warn if a vehicle’s income is negative: Off
* News/Advisors: Warn if a vehicle is lost: Off
* Environment > Industries > Company stations can serve industries with attached neutral stations: Off
* Environment > Cargo distribution: Manual

### Required NewGRFs

* Improved Town Layouts 1.4.0 or later
  * these houses don’t accept Workers or Food, keeping those cargos going only to your industries.

### Recommended NewGRFs

* Iron Horse 2
* Termite (tracks)
* Unsinkable Sam
    * Currently unfinished as of this writing, so I also use Squid Ate Fish
* Mop Expanded Road Vehicles
* Unspooled (roads)
* Av9.8 Aircraft Set
* OpenGFX+ Airports
* Industrial Stations Renewal
* ISR-style Dock
* ISR/DWE-style Objects
* US Stations set
* Total Bridge Renewal Set
* Rainforest Ruins

## Credits
* Beach sprites: [Beach Objects](https://www.tt-forums.net/viewtopic.php?f=26&t=62258) by Quast65, GPL v3 license

## Design Notes

Industries of the Caribbean is an experimental industry/economy mod which aims to radically rethink the OpenTTD economy by breaking common design patterns and reclaiming “useless” features to add interesting gameplay.

Before we get into what I’ve changed, let’s briefly recap how vanilla and most NewGRF economies are structured:

* Money is an early-game constraint, but by mid-game your company earns money faster than you can spend it. The constraint then becomes tile space for stations, junctions, and mainline throughput. OpenTTD would still be fun without money.
* Industries grow to immense production either through station rating-fueled production increases (vanilla), or boost cargos (FIRS). This high production usually requires double-track infrastructure, and don’t even dream of using road vehicles for cargo.
* Most production chains lead to town cargos which are delivered to “black hole” industries, such as Goods, Alcohol, or Vehicles. These are highly profitable, but by the time you complete the production chain to this extent, money is generally not a motivating factor.

The serious OpenTTD players I talk to tend to fall into two gameplay categories:

1. Players who build passenger networks using CargoDist to route passengers automatically and create network design and capacity challenges for gameplay interest.
2. Players who build cargo networks using a complex industry mod like FIRS Steeltown or XIS.

I have played both styles of game and have been frustrated and intrigued by features in each which fall short of interesting gameplay:

* Road vehicles are too low capacity to be useful outside niche roles like boost cargo distribution, feeder lines, or very short distance routes.
* Without daylength patches such as in JGRPP, most rail lines require double track. It would be nice to have some low-traffic branch lines in addition to the heavy trunk lines.
* Ships are so slow that unless you absolutely need them to reach Oil Rigs (vanilla) or Fishing Grounds (FIRS), using them instead of trains often feels silly.
* Passenger transportation gives you nothing but money (a “bad feature,” remember?) and its only gameplay interest comes from fighting to keep up with CargoDist and town growth...which is often more frustrating than fun.
* Endgame town cargos have no incentive to deliver them, and it’s just as profitable to dump them all in one place rather than distributing them across the map.
* Cargo aging and different values per cargo only matter in the early game.
* If you’re not playing with passengers or mail, towns are useless to you and just get in the way.

So, what ~~weird and ill-advised~~ interesting things can we do to change this?

* Primary industries have a fixed production much lower than FIRS, to encourage road vehicles and single-track rail lines to industries while still keeping enough production for busy trunk lines.
* Only primary industries spawn on map generation, and all secondary industries are funded by the player — more on this later. Industries never change production or close, and only Hotels spawn during the game.
* All industries require Workers (Passengers) for production. 
    * Primary industries need a small but steady flow of workers from the nearest town, creating a pleasing network of local roads and bus routes and making towns relevant.
    * Secondary industries need an immense supply of Workers: one per unit of cargo converted. Funding them requires you to think about worker supply and once built, you’ll need to grow cities and run commuter trains from nearby towns and cities.