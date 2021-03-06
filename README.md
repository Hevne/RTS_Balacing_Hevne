# Introduction
My name is Eudald Garrofe, [Hevne](https://github.com/Hevne) on GitHub, I'm a student from CITM's videogames design & development degree. On this website I'm going to talk about the RTS games genre and the main aspects we need to take in account when as a Game Designer we try to balance our game.

# Index

* <a href="#RTS Balance"><b> 1. RTS Balance</b></a>

  * <a href="#RTS Balance difficulty"><b> 1.1 RTS Balance difficulty</b></a>

  * <a href="#How do we test if something is un/balanced?"><b> 1.2 How do we test if something is un/balanced?</b></a>

* <a href="#Tech Trees"><b> 2. Tech Trees</b></a>

  * <a href="#Balacing a Tech Tree"><b> 2.1 Balacing a Tech Tree</b></a>

  * <a href="#Some Tips When Building a Balanced Tech Tree"><b> 2.2 Some Tips When Building a Balanced Tech Tree</b></a>

* <a href="#Resources Gathering"><b> 3. Resources Gathering</b></a>

  * <a href="#Some tips about Balanced Resource Gathering"><b> 3.1 Some tips about Balanced Resource Gathering</b></a>

* <a href="#Game Economy System"><b> 4. Game Economy System</b></a>

  * <a href="#Step 1. Define investment and non-investment resources"><b> 4.1 Main Steps </b></a>

* <a href="#Map Structure"><b> 5. Map Structure</b></a>

  * <a href="#Competitive Maps"><b> 5.1 Competitive Maps</b></a>

    * <a href="#Map Symmetry"><b> 5.1.1 Map Symmetry</b></a>

    * <a href="#Gameplay elements"><b> 5.1.2 Gameplay Elements</b></a>

    * <a href="#Players Route"><b> 5.1.3 Players Route</b></a>
    
  * <a href="#Campaign Maps"><b> 5.2 Campaign Maps</b></a>

* <a href="#Units balancing"><b> 6. Units balancing</b></a>

  * <a href="#Intransitive Mechanics or Rock Paper Scissors"><b> 6.1 Intransitive Mechanics or Rock Paper Scissors</b></a>

    * <a href="#Why Intransitive Mechanics?"><b> 6.1.2 Why Intransitive Mechanics?</b></a>

  * <a href="#Some Maths behind RPS games"><b> 6.2 Some Maths behind RPS games</b></a>

  * <a href="#Tactics taken in account on an RTS"><b> 6.3 Tactics taken in account on an RTS</b></a>

  * <a href="#Solving the human opponent problem"><b> 6.4 Solving the human opponent problem</b></a>
  
* <a href="#AI Balance"><b> 7. AI Balance</b></a>

* <a href="#Sources"><b> 8. Sources</b></a>

<h1 id="RTS Balance"> RTS Balance   </h1>

There can be a misconception that balance is esoteric and only really matters to high level players, but this is far from accurate, since its the keystone to make an RTS game fun.

Which is the intention behind balancing? What does "balancing" even mean? Balacing a game is the action of making the game more fair for each faction, staying as close as possible to a 50/50 win rate. But that's only a small part of the umbrella term of "balance". Balance can be truly defined as **any change to the performance or utility of units and other game components.**

As Game Designers we cannot think about balance as just tweaking numbers, it's about enviosioning and guiding player interactions while providing them with more opportunities to pursue their favourite strategies. Earlier I said that balacing an RTS is the central pillar of making the game fun and to be honest, adding new features is a great way of making an RTS funnier too but they're expensive from a development perspective and additional content is pointless if it's not properly balanced.

What would be the point of having 30 units if only 10 of them are useful?  Having too much content can turn overwhelming for new players to learn, it can lack clarity and can make decisions feel meningless. **Does it really matter which ones I build?**

<br>

![](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/f850d90a-7d5e-48d4-b487-372a169d612b/d6yvl12-1aa5b1ba-2bee-4422-8ab4-daba2fab5047.png/v1/fill/w_2045,h_391,q_70,strp/starcraft___unit_album__ver_54__wip_by_alianys_d6yvl12-pre.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7ImhlaWdodCI6Ijw9MTkwMCIsInBhdGgiOiJcL2ZcL2Y4NTBkOTBhLTdkNWUtNDhkNC1iNDg3LTM3MmExNjlkNjEyYlwvZDZ5dmwxMi0xYWE1YjFiYS0yYmVlLTQ0MjItOGFiNC1kYWJhMmZhYjUwNDcucG5nIiwid2lkdGgiOiI8PTk5MzYifV1dLCJhdWQiOlsidXJuOnNlcnZpY2U6aW1hZ2Uub3BlcmF0aW9ucyJdfQ.2S60GxfWTSgrbtkMY83rjNpuiIfOJJNkNPIkCjN6Plw)

<br>

So first of all one must begin by understanding what it is that makes RTS fun, we can say that the fun of RTS games is the act of **crafting, refining, and executing strategies** Having to gather information and make quick decisions against your opponent is also part of the fun. 

Since RTS contain a wide range of tools as units, upgrades, abilities, buildings and so on, it's up to the player **to piece these tools together in ways that form powerful strategies**, from here we can expect the player having fun but not by the number of tools the player has at hand, instead, we know the player will have fun from combinating these tools, creating his own strategy to defeat the enemy faction.

Pursuing even a simple strategy using the mentioned tools contains lots of depth but if the strategy is countered by an imbalance or an overpowered enemy unit that prevents the player from sticking to his strategy there's no way to respond it, ruining the experience for the player, so here we can see the utility of the game balance.

Meticulous balance creates a richer setting for discovering strategies and for reacting when things don't stick to the player's  plan; if a player's strategy gets countered they might still have a wide arsenal of tools that can perform other functions instead of just being made obsolete.

Good balance doesn't just make an RTS game "more balanced." It emphasizes the unique qualities of each unit and ability, creating more depth and decisions about which tools are used and how they're used.The analogy of RTS as a set of tools for players to utilize encourages design of units that have unique qualities, allowing players to field them under many circumstances for various reasons. Flexible RTS design allows for flexible decision making from players, and meaningful decisions broken up into small increments is at the core of what makes RTS games fun. 

*A game is a series of interesting choices - Sid Meier*

![](https://forums.civfanatics.com/media/civ-6-banner.3815/full)

<h2 id="RTS Balance difficulty"> RTS Balance difficulty   </h2>


RTS games are so difficult to balance, it really turns into a long and iterative proceess, it becomes inevitable to make mistakes along the way when trying to implement our balance into the game. But why is so difficult and we can expect a lot of mistakes during the process? 

The main reason is that we have to take in account **many variables and each context**. Let's give an example using the game Ashes Of The Singularity: Escalation to proof how huge the amount of variables really is.

Let’s assume the Athena and Mauler (Both units of AotS) cost the same resources. Imagine you make them fight, only to find that the Athena wins with 20% of its health left. Does this mean the Athena is overpowered and should be nerfed by 20% to compensate? The Athena might overperform in this one specific case, but does the same thing happen if you get 5 Athenas against 5 Maulers, or 50 against 50? Factors such as reload, burst, and projectile speed can make a massive difference when looking at the scalability of an interaction. Let’s assume even in the 50 v 50 scenario, the Athenas win with a 20% advantage.

![](https://www.stardock.com/ashesofthesingularity/escalation/v275/ashesc_v275_thumb.jpg)

At first glance it can seem safe to state that Athenas are overpowered but unfortunatley for us Game Designers, it's never that simple. You can't just put a bunch of units to engage in a fight and compare their direct interactions, yo need to look at the matchups in their totality and the only way to include known and unknown factors is in regular matches.

Also we have to take into consideration the type of production, the economic management, which factions is fighting against which, the synergy with other unit types, abiities, additional mechanics and a large and so on... Having said that we can take in conclusion that we need to test our balacing features in a real game not just seeing how it performs in a very inaccurate simulation.

<h2 id="How do we test if something is un/balanced?">  How do we test if something is un/balanced?   </h2>

So now we know that we can't fully rely on the data we extract from inaccurate fictitial scenarios where we put two units to fight each other. Now we know we need to test our features in a real game scenario, but we also know that testing is time-consuming and it's difficult to replicate every situation since you need to test the late game in 1v1, 2v2, 3v3, 4v4, different maps, different play styles and skill levels between players. How do we manage to test all these things?

Some ways of testing and gathering data are:

* **Lots of varied play testing:** Try to play variety of maps, play team games, 1v1s, play against a huge variety of players, try different play styles and seek the unbalance.

* **Watching replays and observing:** This one is similar to the playtesting way, but even better since when you are observing a match the emotional investment of winning or losing is thrown out, making it a lot easier to identify what's unfair or not fun.

* **Variety of feedback:** Feedback is a safeguard against making bad decisions. It helps to identify some people you can trust with the quality of feedback and assemble them into beta testing groups. People will suggest things that may have occurred to you but never articulated, or may call you out on an oversight that you never considered.

![](https://www.buildbox.com/wp-content/uploads/2018/08/Game-Development-Forums.jpg)

Even feedback is a very positive and communicative way of finding unbalanced aspects of your game, you can't fully rely on people saying: "This is not fun", "This is unfair" since we have to take in account that these are people who firstly are not happy with some aspect of the game and would like to change it to theis likes. As a Game Designer you must be conscious about how do you envision the game and have a critical vision about which feedback is useful and which differs from your conception of the game. 

Even so, if many players are pointing towards the same issue then it's worth investigating even if you don't think so.

Now that we know which is our work as Game Designers when it comes to balancing, how difficult it is and how to test it, we can move on into different RTS-core features that need a proper balance such as: Units, Maps, Tech Trees, Resources or even AI. 

<h1 id="Tech Trees"> Tech Trees  </h1>

Tech trees can ve conceived as little puzzles that empower the player to personalize the game into something they enjoy, even they use to be simple and isolated tech trees have a very meaningful impact in your game since its going to determine the way the player is going to play and going forward into victory.

Tech trees are a graphic representation of each peace of technology that the game has and how the hierarchy of unlocking each one works.

![](https://steamuserimages-a.akamaihd.net/ugc/23967114491880917/FAAD2CA9F4410BB1A05A3EB5A6DCD991962A5048/)
*Tech Tree of Age Of Empires: The Age of Kings*

Tech trees don't follow an universal set of rules since are directly tied to the nature of the game, even so we can dissect the core aspects of what makes a tech tree a tech tree and these are the nodes.

Each tech tree is composed by connected nodes that form a descendant hierarchy, being the ones at the top of thre hierarchy the lowest tier nodes (easiest to unlock) and the ones at the bottom the highest tier nodes (hardest to unlock). In RTS genre tech trees are usually composed by:

* **Units**
* **Buildings**
* **Units Upgrades**
* **Other: Strictly tied to the nature of the game**

Usually each node has a description for the dynamics that implies unlocking the node.

<h2 id="Balacing a Tech Tree">  Balacing a Tech Tree   </h2>

When balancing a tech tree the most important thing in which as a Game Designer we have to focus is in which moment to allow the creation of every type of unit and upgrade.

First, we should gather all the stuff that we want to be unlocked via the Tech Tree dividing it by Units, Buildings and so on, depending on the nature of your game. Once its done you should put it into a graphic form, as an example I'll use the Tech Tree I designed for my Project II Subject at my career.

![](https://raw.githubusercontent.com/Misioneros-Studio/Mythology-Parade/master/Wiki_pics/Design/research%20tree.png)

Put in into a graphic form, it is clear to see via the scheme how the player will be unlocking stuff during the game, but that's not all since the nature of our game or the conception we have about how it should be will introduce a lot more aspects to take in acount such as:

* **The time needed to unlock each node:** As higher tier the node we're trying to unlock is, the larger ammount of time we should be spending into researching the node.

* **The requiremenets to unlock each node:** Depending on the nature of your own game this will widely vary. In the example of my project game, you need first to have unlocked one of the previous nodes and at the same time dispose of a tokes called: "Sacrifices" or "Blessings". If you are curiours to know more about how my Tech Tree Works click [here](https://github.com/Misioneros-Studio/Mythology-Parade/wiki/Design)

This two aspects are really difficult to really balance since the progression on the Tech Tree will define the pace and the rythm of the game progression feeling. But using the mechanisms I told you about in the Introduction section it will be just a matter of time until you are capable of balancing the progression rate of the Tech Tree. 

Some of the questions that you as a game designer should ask yourself are: Are the players getting x improvement too soon/late? There is a node that's being ignored by the players? Why? Are the unlocked nodes significant and have a real impact on your gameplay?

<h2 id="Some Tips When Building a Balanced Tech Tree">  Some Tips When Building a Balanced Tech Tree   </h2>

* **Know what to acentuate:** Know the gating components of your RTS game, think about the different strategies of the players and how will the Tech Tree impact on those components or strategies. What makes my RTS unique from the rest? Try to accentuate those aspects buffing it with the Tech Tree since your players are playing your game and not another one thanks to those aspects.

* **When should the player be able to get X?:**  Pacing the progression of a tech tree is vital for making it a positive aspect of your game. Lower tier nodes should be simple but potent, hooking the player immediately, in the other hand, higher tiers should add more complex dynamics knowing that the player is ready to understand them.

* **Make the player guess right:** The low level nodes should be an indicative of what the player can expect later if he goes on into a certain brench of the tree. Using as example the tech tree of my Project II, when the tree forks into Lawful/Chaotic paths, the first units are a clear indicative of what kind of brench he is investing his time. 

* **Do more than just give plain power:** Don't just add buffs to your current buildings or units, try to surprise your players constantly with new stuff that makes them truly feel a sense of progression. Increase the core functionalities of the game, don't rely just in numbers!

* **Don't forget your roots:** A common mistake in Tech Trees and also Talent Trees is that the first nodes become uslees when a player reaches the highest tier nodes. As a Game Designer you will want to balance your tech tree such as a big puzzle constantly growing and summing its parts, making each node to have an impact in both early and late game.

<h1 id="Resources Gathering"> Resources Gathering  </h1>

Resource gathering is probably one of the most important mechanics in an RTS game since we use them for researching, building your army and even raising buildings.

Resource gathering systems are very diverse and offer a wide flexibility for the designer to stablish how wants the system to be according to his game conception. Warhammer use resource areas which slowly increase your stock over time, Starcraft have Minerals that can be gathered and so on.

The style of resource gathering in a game will heavily dictate how the game is played, it will create a constant flux for gathering units? or will be more like a king of the hill based system?

![](https://i.pinimg.com/originals/e1/08/91/e1089110c76d068ae4206f26abf4058d.gif)

Gathering systems imply the ability to attack/deny resource gathering of your opponent. This means that we let the door open for a viable strategy for an indirect win rather than immediately. If we keep on destroying the gathering system of our enemy it will lead to our enemy lacking resources to buy/upgrade tools to defeat us, manipulating in that way our opponents income.

At the same time we also let the door open for the player to decide if his strategy will be invest in economy or a rush based one. This helps your game to gain a lot of depth and it means a lot of risk management. The player will have to ask himself how much can he spend on gathering rather than on defending. 

*Although Civilization VI is not an RTS, there are 5 ways to assure your victory (Culture, Science, Economy, Faith or Militar based) This makes the gameplay gain a lot of depth and making the player think about how he is supposed to play according to the circumstances.


<h2 id="Some tips about Balanced Resource Gathering">  Some tips about Balanced Resource Gathering   </h2>

As I said in the last section, resource gathering offers a huge flexibility for the designer and there's not really a way to prove how a resource gathering system is either balanced or unbalanced since this will be determined by the context of the play scenario and how the game is supposed to be.

Some things a designer must take in account when designing a resource system are: 

* **The rarity Index:**  This is about the frequency of resources spawning along the map. Let's assume our game has three types of resources: Wood, Stone and Metal, being the first one the most common one to find and the last one the rarest. Why would we, game designers to create a low-rate spawning resource? High-quality units, the last building improvement and so on... The most common resource will be the one that the player will be needing during the whole match, the rarest resource instead will be the one to provide with the player with the most overpowered tools to defeat the enemy.

* **How many resource types?:** As I said during the introduction, a lot of features don't make the game more interesting and can lead to development high costs and a lack of clarity for new players. How many resource types will your game need to work well with? Don't be shy about cut down heavily the kinds of resources available

* **Finite vs infinite resources:** Infinite resources usually tend to encourage players to wall themselves in turtleing mode and it can led to a boring gameplay since the only way of losing your income would be losing your base. If resources keep running out and force you to migrate throughout the game or expanding your controlled zones, leading to a more interesting, risky and strategy based gameplay.

* **Smooth vs Rough resource income:** Rough resource income is seen on systems that put too much emphasis on worker units, making them expensive and long time steps to gather resources, it can turn annoying since the importance of the gatherer unit is so high.
Smooth resource income however, seen in games such as Starcraft and Warcraft prioritize cheap workers and limit the certain amount of income per minute by restricting the total amount of gathering units. Smooth income based will generate a system where a good player can harvest more than an inexperienced one.

* **Time as a resource:** Any well designed RTS game will take into account the time when producing units or buildings, moving units, gathering other resources and so on... This adds a lot of depth and increases the difficulty of each decision that a player will be forced to make, forcing the player to decide and prioritize on what is he going to do.

![](https://bnetcmsus-a.akamaihd.net/cms/blog_header/bh/BH7HQWEVCV7B1571781106843.jpg)

<h1 id="Game Economy System"> Game Economy System  </h1>

Now that we know the basics for gathering resources is time to talk about the Game Economy. Every RTS game has an internal economy in form of resource gathering and managing these resources. Withouth the game economy system neither the Units, Buildings or Tech Tree would have sense of being.

In spite of the fact that in small companies creation of the game economy often becomes a responsibility of a game designer, economic expertise is extremely important for balancing: it allows to see the big picture, draw parallels with real life utilizing various scientific methodologies.

So, what are the basic steps in creating a balanced in-game economy?

<h3 id="Step 1. Define investment and non-investment resources"> Step 1. Define investment and non-investment resources </h3>

Investment resources are those that influence the speed at which the player receives the main value of the game. Let's assume we need a certain ammount of lumber in order to upgrade our encampment building and in that way speed up our units production time and at the same time we would be speeding up our victory. 

If we talk about non-investment resources following the same example I used before, time would be the non-investment resource since its the resource needed to product a certain ammount of units over time but we cannot use time to reduce the time needed to produce units, it would be kind of Inception.

Usually, resources of all types are described by the game designer at GDD creation, but the game economy designer still needs to carefully check all the mechanics to spot any additional resources that were not taken into account.

<h3 id="Step 2. Build a cost system"> Step 2. Build a cost system </h3>

When making progress, players earn in-game currency or resources that unlock certain content types or new tools for their progression. 

Building a cost system allows you to put correct prices and determine how much everything is worth. For example, a player gets 60 stones for building a quarry on a mountain. How often will they get these 60 stones? At what point in time will they collect, for example, the 3,000 stones needed for a building upgrade? Having such a schedule, the game economy designer adjusts the player's income and expenses for all the in-game resources.

![](https://wowenomics.files.wordpress.com/2009/01/cropped-gold-coins-2.jpg)

<h3 id="Step 3. Create deficit and surplus"> Step 3. Create deficit and surplus </h3>

To engage players we need to let them experience the whole range of emotions, the player won't feel the buzz of victory if he hasn't tasted defeat, since the juice of a game comes from balance between difficult & easy, interesting & boring we can apply the same kind of methodology into our game economy system.

The reaching of maximum profit earnings by the player is similar to the overheated economy, where the game keeps increasing the price of a recently unlocked unit on the tech-tree in order to make the player feel this deficit, but at the same time decreases the price of the first unlocked units, making the player experience a surplus about what before was a deficit.

Let's assume we start our game and to produce a worker we need about 50 wheat, and we produce 0.5 wheat per second. The game goes on and at a certain point we unlock the caravel unit, also we are now producing 5 wheat per second. To build the caraval we need 50 lumber but we are only producing 0.2 lumber per second. The player experiences an surplus when producing workers, giving him a feeling of progression but still lacks resources to build the recent unlocked unit, making him experience a deficit.

<h3 id="Step 4. Decomposition"> Step 4. Decomposition </h3>

The game designer should create dependency plots for a period of time ahead, and break them up into segments and balance them inside these segments (First worker-First caravel ... First caravel-First siege tower ... and so on), getting the zero-sum game as the output. This means that if you count all the total revenues and all expenses, they will add up to 0 and this is an example of a perfectly balanced economy.

<h3 id="So, that's it?"> So, that's it? </h3>

Balacing the game economy can seem like a torturing task to even for the most experienced game designers. However you can adhere to rules, guidelines and models that can help you build your game economy system.

The 4 steps I've covered are a great base for building a balanced game economy, but is important to remember how each game is unique and needs a custom approach which involes continuous monitoring of players behavior.


<h1 id="Map Structure"> Map Structure  </h1>

When it comes to balancing maps on an RTS game and how we should structure them, the most important thing we must take into account is that maps from a competitive-based RTS are so much different from a campaign-based RTS map. So we're going to divide Map Structure into two classes: Competitive and Campaign

Map balancing is probably one of the aspects that requires lest maths working to balance it properly since it's more like about gameplay features, and terrain. Having said that let's get into it. For both competitive and campaign map balance for an RTS, the best way to conceptualize a map is through drawings, diagrams and schemes. Drawings of how the map will be structured, which elements you will use in the map, and how you would dispose them and the routes the player could take. The same goes for schemes and diagrams.

<h2 id="Competitive Maps">  Competitive Maps   </h2>

Competitive maps focus on equality between both players and encouraging both of them in finding each other.

<h3 id="Map Symmetry"> Map Symmetry </h3>

The most important thing and the more differentiating trait about competitive maps structure is **Symmetry**. The most simple, yet most effective way to make a balanced RTS map for a competitve game is to make it symmetrical in order to prevent any player from having an advantage over the other in certain areas.

Also, symmetry is used to avoid unfair advantages at spawning points, supressing in that way things as "Where is he?" If a player knows for sure in which direction he will encounter the enemy base.

*As an example, I'll be illustrating the map symmetry on a map from Blizzard's game Starcraft II.*

![](https://github.com/Hevne/RTS_Balacing_Hevne/blob/master/symmetry.png?raw=true)

Each player starts on one of the corners of the map, being both of them provided with the same ammounts of resources. We can see how the map is really divided into 4 symmetrycal quads. 

<h3 id="Gameplay elements"> Gameplay elements </h3>

Gameplay elements follow the symmetric structure of the map, being scattered around it following a symmetric pattern, the symmetrical distribution of these elements assures that any player is going to have an avantage over the other when it comes to resource gathering. Even elements as the tallgrass (hide zones) or the observatories (watch points) are symmetrical in that way.

The map designer should set the resources in a way that encourages the players to slowly go towards each other. That can be seen in the bonus resources areas (Rich Mineral) in order to force a combat engage between both players

![](https://github.com/Hevne/RTS_Balacing_Hevne/blob/master/Map%20gmply.png?raw=true)

However, things such as textures, backgrounds or decorative tiles which designers call "non gameplay elements" should'nt be symmetrical at all, since that would give an artificial feeling for the players during the game. Specially we can see this in the background of this particular map.

<h3 id="Players Route"> Players Route </h3>

For achieving succesfully the crafting of a map, the most useful tools to use are squetches and schemes. Squetches are incredibly important to assure that the map and gameplay elements of the map are symmetrical, and for drawing the possible paths that players could take

![](https://github.com/Hevne/RTS_Balacing_Hevne/blob/master/PACE.png?raw=true)

<h2 id="Campaign Maps">  Campaign Maps   </h2>

When talking about campaign maps its important to keep focused on presenting clear objectives to the player and also giving a sense of progression through the map. For campaign maps there is no need to be symmetrical since you are fighting against an AI and if you are on advantage or disadvantage would be the decision of the game designer.

The player must be encouraged by his progression, feel empowered at each step he takes while trying to fulfill the main objective of the map. For Illustrating this I'm gonna be using a map from Warcraft II called Badlands.

![](https://github.com/Hevne/RTS_Balacing_Hevne/blob/master/MAPWCFT.png?raw=true)

First of all we can see how the gameplay elements of the map aren't symmetrical anymore and the terrain is build in a more scattered way, encouraging the players to explore and giving them a bigger sense of discovering.

The goal or objective that is presented to the player is to escort Cho'Gall (A Warcraft character) to Grim'Batol, in order to accomplish this task the player will have to destroy the Alliance fortresses that separate him from Grim'Batol. The player can choose between different paths and strategies in order to accomplish that making him feel great and intelligent when fulfilling the objective but the truth is that the one guiding him is the map designer.

We can see how are certain zones which main use is to be built on, creating a feeling of progression through the map for the player.


<h1 id="Units balancing"> Units balancing  </h1>

Units balancing is one of the core things we need to priorize when balancing our game since it will determine which outcome will have every engaged fight between two players. Although it can seem that units balancing is just about setting numbers, strengths and weaknesses is a bit more complex than just that.

Units should have multiple facets that determine their utility and why a player would want to build them. Using again as an example Ashes of the Singularity, the Archer is a unit designed to counter the Athena, but they're embedded within a more detailed context. The Athena is a cruiser which costs both Metal and Radioactives (both resources of the game), while the Archer is a frigate which only costs Metal, allowing it to be used more flexibly to complement Radioactives-heavy strategies or to burn excess Metal if your Radioactives income suddenly drops. Frigates are also considerably faster than cruisers, which makes Archers useful as a nimble form of harassment. 
Archers have high damage but low health, which makes them great against buildings, but vulnerable versus Orbitals and area of effect damage. 

We can see how balacing the resources needed to produce each unit is too a core component of units mechanic, in that way we let the door open for the player to create his own strategy not only focused on countering units.

Having said that, I'm going to cover how to balance the units combat system based on RPS (Rock Papers Scissors) base.

<h2 id="Intransitive Mechanics or Rock Paper Scissors"> Intransitive Mechanics or Rock Paper Scissors  </h2>

"Rock-Paper-Scissors like game" these are the games which don't have a single dominant strategy, because everything is weak and strong at the same time against something else, a kind of zer-sum games.

Intransitive mechanics can be found constantly in any kind of games. In fighting games is a common pattern that normal attacks are weak against a block, block are weak against throws and throws weak against attacks. In Real time strategy games, RTS, we see too a common pattern in which fliers defeat infantry, infantry is strong against archers and archers are a good choice to shoot at fliers.

Sometimes this relation is not that obvious, for example in a game as League Of Legends in which we have different kind of champions for the jungle role, (Tanks, assassins, fighters...) Its not so obvious to see which kind of champion is strong against which but we can certainly stablish a pattern. Tanks>Assassins, Assassins>Fighters, Fighters>Tanks. A lot of times the current state of the meta and of the maths behind each champion states which is the current relation for the rock papers scissors formula.

Another not so clear example is a game in which one kind of unit is an expert in long-range attacks, having advantage over short-range attack units. But a short-range attacker which has the ability of turning invisible or moving really fast across the map can counter this range advantage by making the long-range unit weak against attacks.


![](https://www.pngitem.com/pimgs/m/266-2667284_rock-paper-scissors-diagram-hd-png-download.png)

<h3 id="Why Intransitive Mechanics?"> Why Intransitive Mechanics?  </h3>

So why if all intransitive mechanics are improved and modified versions of Rock-Paper-Sicssors, what's the appeal? 

First, an intransitive game is by far more interesting that one which only has in account one way or a single dominant strategy, going all in with Rock for example would tend to be boring and tedious for most of player, Intransitive mechanics present more variety in lay and make it more interesting.

For another, an intransitive mechanic always allows players to change or modify the way they are playing the game until now and changing their strategies in mid-game. In this way players can decide certain choics in light of what they have seen doing other rival players, in this way you can react in a space of few milliseconds.

Furthermore, intransitive mechanics serve as an "emergency brake" on runaway dominant strategies. Even if you're not sure about which is the best strategy in your game, making all the strategies have an intransitive relationship you can know that there will not be just a single dominant strategies above the rest. 

Intransitive mechanics can be tangled as much as the designer wants to but its better to keep it simple for the player having the classic formula of a relation between 3 used in games as Pokemon, Starcraft, Civilization or even Dark Souls. Just imagine playing a game and having to take in account all these relations:

![](https://retrohelix.com/en/wp-content/uploads/2013/08/rps11.jpg)

<h2 id="Some Maths behind RPS games"> Some Maths behind RPS games </h2>

So if we propose a table in which we take in account the possible throws of each player we can start doing some mathy-things with this. Calling our rival’s throws r, p and s, and our throws R, P and S. 

Since winning and losing are equal and opposite and draws are right in the middle, let’s call a win +1 point, a loss -1 point, and a draw 0 points:

| - | r | p | s |
| -- | -- | -- | -- |
| R | +0 | -1 | +1|
| P | +1 |+0 | -1|
|S | -1| +1| +0|


Now if we re-frame this table by calling r, p and s the probabilites of the opponent for each possible throw. For example, let's assume that you know in advance that your rival is currently using a strategy based on a probability r=0.5, p=s=0.25 This meaning that by every paper or scissor he throws two rocks. What’s the best counter-strategy to come up with?

To answer that question, we can construct a set of three equations that tells you your payoffs for each throw using the table constructed before.

|Payoffs|
|---|
|<a href="https://www.codecogs.com/eqnedit.php?latex=R&space;=&space;0r&space;&plus;&space;(-1)p&space;&plus;&space;1s&space;=&space;s-p" target="_blank"><img src="https://latex.codecogs.com/gif.latex?R&space;=&space;0r&space;&plus;&space;(-1)p&space;&plus;&space;1s&space;=&space;s-p" title="R = 0r + (-1)p + 1s = s-p" /></a>|
|<a href="https://www.codecogs.com/eqnedit.php?latex=P&space;=&space;1r&space;&plus;&space;0p&space;&plus;&space;(-1)s&space;=&space;r-s" target="_blank"><img src="https://latex.codecogs.com/gif.latex?P&space;=&space;1r&space;&plus;&space;0p&space;&plus;&space;(-1)s&space;=&space;r-s" title="P = 1r + 0p + (-1)s = r-s" /></a>|
|<a href="https://www.codecogs.com/eqnedit.php?latex=S&space;=&space;(-1)r&space;&plus;&space;1p&space;&plus;&space;0s&space;=&space;p-r" target="_blank"><img src="https://latex.codecogs.com/gif.latex?S&space;=&space;(-1)r&space;&plus;&space;1p&space;&plus;&space;0s&space;=&space;p-r" title="S = (-1)r + 1p + 0s = p-r" /></a>|


So based on the probabilities, you can calculate the payoffs. In the case of our rock-heavy opponent, the payoffs are:
* <a href="https://www.codecogs.com/eqnedit.php?latex=R=0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?R=0" title="R=0" /></a>

* <a href="https://www.codecogs.com/eqnedit.php?latex=P=0.25" target="_blank"><img src="https://latex.codecogs.com/gif.latex?P=0.25" title="P=0.25" /></a>

* <a href="https://www.codecogs.com/eqnedit.php?latex=S=-0.25" target="_blank"><img src="https://latex.codecogs.com/gif.latex?S=-0.25" title="S=-0.25" /></a>

Since P is he throw with the biggest payoff of all three throws and assuming that the opponent strategy is not going to change at all during the match our best counter-strategy will be to throw Paper every time, being this strategy the most efficient and effective of them all. Meaning that we would gain 0.25 per throw, this meaning that for every 4 throws we will win one more game than we lose.

In fact, we’ll find that if our opponent merely throws rock the tiniest, slightest bit more often than the others, the net payoff for P will be better than the others, and our best strategy is still to throw Paper 100% of the time, until our opponent modifies their strategy. 

This is significant; it tells us that an intransitive mechanic is very fragile, and that even a slight imbalance on the player’s part can lead to a completely dominant strategy on the part of the opponent.

Of course, against a human opponent who notices we’re always throwing P, their counter-strategy would be to throw a greater proportion of s, which then forces us to throw some R, which then causes them to throw p, which makes us throw S, which makes them throw r, and around and around we go. 

<h2 id="Tactics taken in account on an RTS"> Tactics taken in account on an RTS </h2>

How much strategy is needed in an RTS to win a human opponent? Assuming that RTSs can be simplified to the Rock-Paper-Scissors (RPS) formula makes this last question a lot easier to answer since a chinese university has found the always-winning strategy for an RPS based game.

Is stated that if a player wins over her opponent in one play, her probability of repeating the same action in the next play is considerably higher than her probabilities of shifting actions. 

If a player has lost two or more times, she is likely to shift her play, and more likely to shift to the play that will beat the one that has just beaten her than the same one her opponent just used to beat her.

So its clear that if a player takes in account this method when confronting another player he has a significantly higher rate of winning since he can constantly predict the movements or strategy that will follow the other player in order to beat him.

If I'm Alex and my rival is Paul, Paul has been trying to destroy my tanks using infantry units and by now his troops has been oblittered so he is more likely to start producig anti-tank troops, knowing this I can anticipate and prepare infantry units to counter his anti-tank troops.

![](https://qph.fs.quoracdn.net/main-qimg-5f2c081d0d447b96b6fc74a2bb71ae98.webp) 

But as I stated before: two conscious and gamer players can be engaged on a constant loop if following this strategy so, how to solve this situation?

<h2 id="Solving the human opponent problem"> Solving the human opponent problem </h2>

Rock-Paper-Scissors is a symmetric zero-sum game, so:

<a href="https://www.codecogs.com/eqnedit.php?latex=R&space;=&space;P&space;=&space;S&space;=&space;0" target="_blank"><img src="https://latex.codecogs.com/gif.latex?R&space;=&space;P&space;=&space;S&space;=&space;0" title="R = P = S = 0" /></a>

Since the opponent must select exactly one throw, we also know the probabilities of their throw add up to 100%:

<a href="https://www.codecogs.com/eqnedit.php?latex=r&space;&plus;&space;p&space;&plus;&space;s&space;=&space;1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?r&space;&plus;&space;p&space;&plus;&space;s&space;=&space;1" title="r + p + s = 1" /></a>

From here we can solve the system of linear equations by substitution using the known values from our previous <a href="#Some Maths behind RPS games"><b>table</b></a>



* <a href="https://www.codecogs.com/eqnedit.php?latex=R=&space;0&space;=&space;s-p&space;\Rightarrow&space;p=s" target="_blank"><img src="https://latex.codecogs.com/gif.latex?R=&space;0&space;=&space;s-p&space;\Rightarrow&space;p=s" title="R= 0 = s-p \Rightarrow p=s" /></a>

* <a href="https://www.codecogs.com/eqnedit.php?latex=P&space;=&space;0&space;=&space;r-s&space;\Rightarrow&space;r=s" target="_blank"><img src="https://latex.codecogs.com/gif.latex?P&space;=&space;0&space;=&space;r-s&space;\Rightarrow&space;r=s" title="P = 0 = r-s \Rightarrow r=s" /></a>

* <a href="https://www.codecogs.com/eqnedit.php?latex=S&space;=&space;0&space;=&space;p-r&space;\Rightarrow&space;p=r" target="_blank"><img src="https://latex.codecogs.com/gif.latex?S&space;=&space;0&space;=&space;p-r&space;\Rightarrow&space;p=r" title="S = 0 = p-r \Rightarrow p=r" /></a>

* <a href="https://www.codecogs.com/eqnedit.php?latex=r&plus;p&plus;s&space;=&space;r&plus;r&plus;r&space;=&space;1&space;\Rightarrow&space;r=1/3" target="_blank"><img src="https://latex.codecogs.com/gif.latex?r&plus;p&plus;s&space;=&space;r&plus;r&plus;r&space;=&space;1&space;\Rightarrow&space;r=1/3" title="r+p+s = r+r+r = 1 \Rightarrow r=1/3" /></a>

* <a href="https://www.codecogs.com/eqnedit.php?latex=r=p=s&space;\Rightarrow&space;p=1/3,&space;s=1/3" target="_blank"><img src="https://latex.codecogs.com/gif.latex?r=p=s&space;\Rightarrow&space;p=1/3,&space;s=1/3" title="r=p=s \Rightarrow p=1/3, s=1/3" /></a>

By looking at this solved system of equations we can see how our solution is that the opponent should throw r, p and s each with probabilities of 1/3. So we can say that against a completely random opponent it doesn't matter what we choose since our odds of winning or losing are the same in all ways.

So assuming that our opponent knows this too, if we choose an unbalanced strategy not based on this 1/3 for each possible throw our opponent can alter his throw ratio to beat us, so the best option for us is to stick with the 1/3 probability strategy.

***This doesn't mean that in actual play we should choose a completely random strategy to win***

When humans try to play a game randomly they tend to not be quite good at it, so in the real world the best and optimal strategy is to keep an equal throw ratio for each possible option, but at the same time be constantly evaluating your opponents patterns and play style in order to exploit it in your favour and masking any kind of pattern in your own play.

So the solution of 1:1:1 does not say which throw you must choose at any given time **(that is in fact where the skill of the game comes in)**, but just that over time we expect the optimal strategy to be a 1:1:1 ratio (because any deviation from that hands your opponent a strategy that wins more often over you until you readjust your strategy back to 1:1:1).

<h1 id="AI Balance"> AI Balance </h1>

AI Balance is a core aspect when talking about balance on an RTS since if the AI is not correctly balanced according to all the features of your game the balance done previously can become useless. Is your AI not competent enough? It turns out to be a nightmare for your players? Why? How to solve these things?

First of all is important to determine the grade of difficulty you want your AI to be. It's common to see different AI difficulties for the player to choose before starting a game in order to let the player adjust the grade of difficulty for the match, now we are going to talk about some tools that can be used in order to balance your AI according to the difficulty set by the player.

But first, how is your AI supposed to work? How it will react to certain inputs? Which would be its outputs? For this, we should first stablish a State Machine Diagram in order to portray the basics of the behavior of the AI, something like this one:

![](https://valdiviadev.github.io/RTS-balancing-research/Images/StateMachine.png)

How will a worker unit react if being attacked by the player? It should flee seeking for aid in some city, an archer should probably find a group of soldiers to be covered and have free fire towards the player, etc... Making a more "intelligent" AI it will mean making a harder hone too since the reactions of the AI will determine how easy is for the player to win the game. As more complex and realistic reactions, it will be harder for the player.

As I said before, now I'm going to cover some of the most common ways to balance AIs used on RTS:

* Have all factions/races be the same but with different appearance.

* Have the factions/races be different but make sure that there exists a RPS relation between them.

* Just don't balance them and let some factions/races be more difficult to beat

The developers can too tweak some numbers in the AI code in order to make it harder or easier, for example: decreasing production rate, decrease resource gathering rate, increasing times of production and vice versa. 

A common way to determine the grade of difficulty of an AI is to stablish a pattern of conduct, giving the AI a task-list that is well known by the designer that is the best way to win a match, making the AI rush certain buildings or units while the player is still thinking about its strategy.

And finally but not my favourite is to make the AI cheat, some examples of these cheap tricks could be:

* No fog of war for the AI

* AI knows what you are producing and builds to counter it

* They start with more resources and collect it faster

To finish, AI is quite hard to balance since it depends on a highly consistent and usually playtesting applying a lot of different play styles, but it's not just "balanced" or "unbalanced" it's about if it really fits into the global game and if it's properly adjusted to the difficulty the player is expecting.

<h1 id="Sources"> Sources </h1>

***About General Balancing***

* [Why Balance Matters](https://www.stardock.com/games/article/487836/dev-journal-why-balance-matters)

* [The Challenge of Balancing an RTS](https://www.stardock.com/games/article/487949/dev-journal-the-challenge-of-balancing-an-rts)

* [Asymmetric Design](https://www.youtube.com/watch?v=F1w-qCbYVe8)

* [What Makes RTS Fun](https://gamecloud.net.au/features/opinion/what-makes-rts-games-fun-the-challenge-of-balancing-an-rts)

* [The Balance Between Power Progression and Equilibrium](https://www.gamasutra.com/blogs/BrandonCasteel/20170306/292982/The_Balance_of_Power_Progression_and_Equilibrium_in_RealTime_StrategyGames.php)

***About Tech Trees***

* [A Spec Into Tech Trees](https://gamedevelopment.tutsplus.com/articles/lets-spec-into-talent-trees-a-primer-for-game-designers--gamedev-6691)

* [Creating And Adaptative Tech Tree](https://www.gamasutra.com/view/news/341477/Game_Design_Deep_Dive_Creating_an_adaptive_tech_tree_in_Dawn_of_Man.php)

* [Tech Tree Composition](https://books.google.es/books?id=RhVoR-ATDlUC&pg=PT251&lpg=PT251&dq=tech+tree+balancing&source=bl&ots=b55nW0D4G-&sig=oTwLejX0L3NGmAfw2_93jd--E1E&hl=es&sa=X&ved=0ahUKEwjW1I2suLXZAhVmneAKHfR5Cro4ChDoAQhsMAk#v=onepage&q=tech%20tree%20balancing&f=true)

***About Resource Gathering***

* [Discussion About Resource Gathering](https://www.gamedev.net/forums/topic/440191-rts-what-is-your-favorite-resource-system/)

* [Thoughts On Resource Management](https://waywardstrategy.com/2014/12/18/random-thoughts-on-resource-management-in-rts/)

* [Resource Gathering Styles](https://www.reddit.com/r/truegaming/comments/n9q0z/strategy_in_rts_resource_gathering_styles/)

***About Economy System***

* [Basic Steps Of an Economy System](https://www.gamasutra.com/blogs/DarinaEmelyantseva/20190418/340987/5_Basic_Steps_in_Creating_Balanced_InGame_Economy.php)

***About Map Structure***

* [Properties Of Good RTS Level Design](https://gamedev.stackexchange.com/questions/2370/properties-of-good-rts-level-design)

* [Multiplayer Map Design](https://waywardstrategy.com/2015/06/07/time-as-a-resource-part-2-multiplayer-map-design/)

* [Beginner's Guide To Level Design](https://gamedevelopment.tutsplus.com/tutorials/a-beginners-guide-to-designing-video-game-levels--cms-25662)

***About Units***

* [The Balance of Power: Progression and Equilibrium in Real-Time Strategy Games](https://www.gamasutra.com/blogs/BrandonCasteel/20170306/292982/The_Balance_of_Power_Progression_and_Equilibrium_in_RealTime_StrategyGames.php)

* [Intransitive Mechanics](https://gamebalanceconcepts.wordpress.com/2010/09/01/level-9-intransitive-mechanics/)

* [Examining the Implementation of Rock, Paper, Scissors, Balance in Video Games](https://www.youtube.com/watch?v=N69Jzzcu57Q)

* [Perfect Imbalance](https://www.youtube.com/watch?v=e31OSVZF77w)

* [Applying RPS to games](https://www.gamasutra.com/blogs/DevonWiersma/20170428/297030/Applying_Rock_Paper_Scissors_to_Video_Games.php)

* [Introduction About Units Balance](http://www.oxeyegames.com/rts-game-play-part-5-introduction-to-unit-balancing/)

***About AI***

* [How AI is balanced on RTS games?](https://gamedev.stackexchange.com/questions/127779/how-ai-is-balanced-across-different-type-of-races-in-rts-games)

