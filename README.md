# Introduction
My name is Eudald Garrofe, I'm a student from CITM's videogames design & development degree. On this website I'm going to talk about the RTS games genre and the main aspects we need to take in account when as a Game Designer we try to balance our game.

## RTS Balance 
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

### RTS Balance difficulty

RTS games are so difficult to balance, it really turns into a long and iterative proceess, it becomes inevitable to make mistakes along the way when trying to implement our balance into the game. But why is so difficult and we can expect a lot of mistakes during the process? 

The main reason is that we have to take in account **many variables and each context**. Let's give an example using the game Ashes Of The Singularity: Escalation to proof how huge the amount of variables really is.

Let’s assume the Athena and Mauler (Both units of AotS) cost the same resources. Imagine you make them fight, only to find that the Athena wins with 20% of its health left. Does this mean the Athena is overpowered and should be nerfed by 20% to compensate? The Athena might overperform in this one specific case, but does the same thing happen if you get 5 Athenas against 5 Maulers, or 50 against 50? Factors such as reload, burst, and projectile speed can make a massive difference when looking at the scalability of an interaction. Let’s assume even in the 50 v 50 scenario, the Athenas win with a 20% advantage.

![](https://www.stardock.com/ashesofthesingularity/escalation/v275/ashesc_v275_thumb.jpg)

At first glance it can seem safe to state that Athenas are overpowered but unfortunatley for us Game Designers, it's never that simple. You can't just put a bunch of units to engage in a fight and compare their direct interactions, yo need to look at the matchups in their totality and the only way to include known and unknown factors is in regular matches.

Also we have to take into consideration the type of production, the economic management, which factions is fighting against which, the synergy with other unit types, abiities, additional mechanics and a large and so on... Having said that we can take in conclusion that we need to test our balacing features in a real game not just seeing how it performs in a very inaccurate simulation.

### How do we test if something is un/balanced?

So now we know that we can't fully rely on the data we extract from inaccurate fictitial scenarios where we put two units to fight each other. Now we know we need to test our features in a real game scenario, but we also know that testing is time-consuming and it's difficult to replicate every situation since you need to test the late game in 1v1, 2v2, 3v3, 4v4, different maps, different play styles and skill levels between players. How do we manage to test all these things?

Some ways of testing and gathering data are:

* Lots of varied play testing: Try to play variety of maps, play team games, 1v1s, play against a huge variety of players, try different play styles and seek the unbalance.

* Watching replays and observing: This one is similar to the playtesting way, but even better since when you are observing a match the emotional investment of winning or losing is thrown out, making it a lot easier to identify what's unfair or not fun.

* Variety of feedback: Feedback is a safeguard against making bad decisions. It helps to identify some people you can trust with the quality of feedback and assemble them into beta testing groups. People will suggest things that may have occurred to you but never articulated, or may call you out on an oversight that you never considered.

Even feedback is a very positive and communicative way of finding unbalanced aspects of your game, you can't fully rely on people saying: "This is not fun", "This is unfair" since we have to take in account that these are people who firstly are not happy with some aspect of the game and would like to change it to theis likes. As a Game Designer you must be conscious about how do you envision the game and have a critical vision about which feedback is useful and which differs from your conception of the game. 

Even so, if many players are pointing towards the same issue then it's worth investigating even if you don't think so.

![](https://www.buildbox.com/wp-content/uploads/2018/08/Game-Development-Forums.jpg)

# Resources Gathering
Resource gathering is probably one of the most important mechanics in an RTS game since we use them for researching, building your army and even raising buildings.

Resource gathering systems are very diverse and offer a wide flexibility for the designer to stablish how wants the system to be according to his game conception. Warhammer use resource areas which slowly increase your stock over time, Starcraft have Minerals that can be gathered and so on.

The style of resource gathering in a game will heavily dictate how the game is played, it will create a constant flux for gathering units? or will be more like a king of the hill based system?

![](https://i.pinimg.com/originals/e1/08/91/e1089110c76d068ae4206f26abf4058d.gif)

Gathering systems imply the ability to attack/deny resource gathering of your opponent. This means that we let the door open for a viable strategy for an indirect win rather than immediately. If we keep on destroying the gathering system of our enemy it will lead to our enemy lacking resources to buy/upgrade tools to defeat us, manipulating in that way our opponents income.

At the same time we also let the door open for the player to decide if his strategy will be invest in economy or a rush based one. This helps your game to gain a lot of depth and it means a lot of risk management. The player will have to ask himself how much can he spend on gathering rather than on defending. 

*Although Civilization VI is not an RTS, there are 5 ways to assure your victory (Culture, Science, Economy, Faith or Militar based) This makes the gameplay gain a lot of depth and making the player think about how he is supposed to play according to the circumstances.

## Some tips about Resource Gathering 
As I said in the last section, resource gathering offers a huge flexibility for the designer and there's not really a way to prove how a resource gathering system is either balanced or unbalanced since this will be determined by the context of the play scenario and how the game is supposed to be.

Some things a designer must take in account when designing a resource system are: 
* The rarity Index:  This is about the frequency of resources spawning along the map. Let's assume our game has three types of resources: Wood, Stone and Metal, being the first one the most common one to find and the last one the rarest. Why would we, game designers to create a low-rate spawning resource? High-quality units, the last building improvement and so on... The most common resource will be the one that the player will be needing during the whole match, the rarest resource instead will be the one to provide with the player with the most overpowered tools to defeat the enemy.

*

# Index
Now that we know which is our work as Game Designers, how difficult it is and how to do it we can move on into different RTS-core features as: Units, map, skill trees, or resources:

* <a href="#Intransitive Mechanics or Rock Paper Scissors"><b> 1. Intransitive Mechanics or Rock Paper Scissors</b></a>
* <a href="#Why Intransitive Mechanics?"><b> 1.2. Why Intransitive Mechanics?</b></a>
* <a href="#Some Maths behind RPS games"><b> 2. Some Maths behind RPS games</b></a>
* <a href="#Tactics taken in account on an RTS"><b> 3. Tactics taken in account on an RTS</b></a>
* <a href="#Solving the human opponent problem"><b> 4. Solving the human opponent problem</b></a>
* <a href="#Bibliography"><b> 5. Bibliography</b></a>

# Units balancing

Units balancing is one of the core things we need to priorize when balancing our game since it will determine which outcome will have every engaged fight between two players. Although it can seem that units balancing is just about setting numbers, strengths and weaknesses is a bit more complex than just that.

Units should have multiple facets that determine their utility and why a player would want to build them. Using again as an example Ashes of the Singularity, the Archer is a unit designed to counter the Athena, but they're embedded within a more detailed context. The Athena is a cruiser which costs both Metal and Radioactives (both resources of the game), while the Archer is a frigate which only costs Metal, allowing it to be used more flexibly to complement Radioactives-heavy strategies or to burn excess Metal if your Radioactives income suddenly drops. Frigates are also considerably faster than cruisers, which makes Archers useful as a nimble form of harassment. 
Archers have high damage but low health, which makes them great against buildings, but vulnerable versus Orbitals and area of effect damage. 

We can see how balacing the resources needed to produce each unit is too a core component of units mechanic, in that way we let the door open for the player to create his own strategy not only focused on countering units.

Having said that, I'm going to cover how to balance the units combat system based on RPS (Rock Papers Scissors) base.

<h1 id="Intransitive Mechanics or Rock Paper Scissors"> Intransitive Mechanics or Rock Paper Scissors  </h1>

"Rock-Paper-Scissors like game" these are the games which don't have a single dominant strategy, because everything is weak and strong at the same time against something else, a kind of zer-sum games.

Intransitive mechanics can be found constantly in any kind of games. In fighting games is a common pattern that normal attacks are weak against a block, block are weak against throws and throws weak against attacks. In Real time strategy games, RTS, we see too a common pattern in which fliers defeat infantry, infantry is strong against archers and archers are a good choice to shoot at fliers.

Sometimes this relathion is not that obvious, for example in a game as League Of Legends in which we have different kind of champions for the jungle role, (Tanks, assassins, fighters...) Its not so obvious to see which kind of champion is strong against which but we can certainly stablish a pattern. Tanks>Assassins, Assassins>Fighters, Fighters>Tanks. A lot of times the current state of the meta and of the maths behind each champion states which is the current relation for the rock papers scissors formula.

Another not so clear example is a game in which one kind of unit is an expert in long-range attacks, having advantage over short-range attack units. But a short-range attacker which has the ability of turning invisible or moving really fast across the map can counter this range advantage by making the long-range unit weak against attacks.


![](https://www.pngitem.com/pimgs/m/266-2667284_rock-paper-scissors-diagram-hd-png-download.png)

<h2 id="Why Intransitive Mechanics?"> Why Intransitive Mechanics?  </h2>

So why if all intransitive mechanics are improved and modified versions of Rock-Paper-Sicssors, what's the appeal? 

First, an intransitive game is by far more interesting that one which only has in account one way or a single dominant strategy, going all in with Rock for example would tend to be boring and tedious for most of player, Intransitive mechanics present more variety in lay and make it more interesting.

For another, an intransitive mechanic always allows players to change or modify the way they are playing the game until now and changing their strategies in mid-game. In this way players can decide certain choics in light of what they have seen doing other rival players, in this way you can react in a space of few milliseconds.

Furthermore, intransitive mechanics serve as an "emergency brake" on runaway dominant strategies. Even if you're not sure about which is the best strategy in your game, making all the strategies have an intransitive relationship you can know that there will not be just a single dominant strategies above the rest. 

Intransitive mechanics can be tangled as much as the designer wants to but its better to keep it simple for the player having the classic formula of a relation between 3 used in games as Pokemon, Starcraft, Civilization or even Dark Souls. Just imagine playing a game and having to take in account all these relations:

![](https://retrohelix.com/en/wp-content/uploads/2013/08/rps11.jpg)

<h1 id="Some Maths behind RPS games"> Some Maths behind RPS games </h1>

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

<h1 id="Tactics taken in account on an RTS"> Tactics taken in account on an RTS </h1>

How much strategy is needed in an RTS to win a human opponent? Assuming that RTSs can be simplified to the Rock-Paper-Scissors (RPS) formula makes this last question a lot easier to answer since a chinese university has found the always-winning strategy for an RPS based game.

Is stated that if a player wins over her opponent in one play, her probability of repeating the same action in the next play is considerably higher than her probabilities of shifting actions. 

If a player has lost two or more times, she is likely to shift her play, and more likely to shift to the play that will beat the one that has just beaten her than the same one her opponent just used to beat her.

So its clear that if a player takes in account this method when confronting another player he has a significantly higher rate of winning since he can constantly predict the movements or strategy that will follow the other player in order to beat him.

If I'm Alex and my rival is Paul, Paul has been trying to destroy my tanks using infantry units and by now his troops has been oblittered so he is more likely to start producig anti-tank troops, knowing this I can anticipate and prepare infantry units to counter his anti-tank troops.

![](https://qph.fs.quoracdn.net/main-qimg-5f2c081d0d447b96b6fc74a2bb71ae98.webp) 

But as I stated before: two conscious and gamer players can be engaged on a constant loop if following this strategy so, how to solve this situation?

<h1 id="Solving the human opponent problem"> Solving the human opponent problem </h1>

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

<h1 id="Bibliography"> Bibliography </h1>

* [The Balance of Power: Progression and Equilibrium in Real-Time Strategy Games](https://www.gamasutra.com/blogs/BrandonCasteel/20170306/292982/The_Balance_of_Power_Progression_and_Equilibrium_in_RealTime_StrategyGames.php)
* [Intransitive Mechanics](https://gamebalanceconcepts.wordpress.com/2010/09/01/level-9-intransitive-mechanics/)
* [Examining the Implementation of Rock, Paper, Scissors, Balance in Video Games](https://www.youtube.com/watch?v=N69Jzzcu57Q)
* [Perfect Imbalance](https://www.youtube.com/watch?v=e31OSVZF77w)
* [Applying RPS to games](https://www.gamasutra.com/blogs/DevonWiersma/20170428/297030/Applying_Rock_Paper_Scissors_to_Video_Games.php)

