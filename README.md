# RTS_Balacing_Hevne


- Units: Combat, building?
# Units Balacing

Units and unit management are one of the core components of any RTS video game. To make the combat in RTS games engaging, it is important to have a balanced roster of units. Without a good unit balance, the strategy part of a real time strategy game would fall flat, and the game would not feel as a strategy game, but something like a construction simulation game with units that eliminate each other.

## Intransitive Mechanics or Rock Paper Scissors (RPS)

Intransitive Mechanics is just a geeky way of saying "Rock-Paper-Scissors like game" these are the games which don't have a single dominant strategy, because everything is weak and strong at the same time against something else, a kind of zer-sum games.

We see intransitive mechanics in games all the time. In fighting games, a typical pattern is that normal attacks are defeated by blocks, blocks are defeated by throws, and throws are defeated by attacks. In real-time strategy games, a typical pattern is that you have fliers that can destroy infantry, infantry that works well against archers, and archers are great at bringing down fliers.

Some of these relationships might not be immediately obvious. For example, consider a game where one kind of unit has long-range attacks, which is defeated by a short-range attacker who can turn invisible; this in turn is defeated by a medium-range attacker with radar that reveals invisible units; and the medium-range attacker is of course weak against the long-range attacker.

![](https://github.com/Hevne/RTS_Balacing_Hevne/blob/master/rps.png)

## Why Intransitive Mechanics?

It may be worth asking, if all intransitive mechanics are just glorified versions of Rock-Paper-Scissors, what’s the appeal? Few people play Rock-Paper-Scissors for fun, so why should they enjoy a game that just uses the same mechanics and dresses them differently?

For one thing, an intransitive game is at least more interesting than one with a single dominant strategy (“Rock-Rock-Rock”) because you will see more variety in play. For another, an intransitive mechanic embedded in a larger game may still allow players to change or modify their strategies in mid-game. Players may make certain choices in light of what they observe other players doing now (in real-time), particularly in action-based games where you must react to your opponent’s reaction to your reaction to their action in the space of a few milliseconds.


Additionally, intransitive mechanics serve as a kind of “emergency brake” on runaway dominant strategies. Even if you don’t know exactly what the best strategy in your game is, if all strategies have an intransitive relationship, you can at least know that there will not be a single dominant strategy that invalidates all of the others, because it will be weak against at least one other counter-strategy. 

## Some Maths behind RPS games

First, let’s look at the outcomes. Let’s call our opponent’s throws r, p and s, and our throws R, P and S. Since winning and losing are equal and opposite (that is, one win + one loss balances out) and draws are right in the middle, let’s call a win +1 point, a loss -1 point, and a draw 0 points:

| - | r | p | s |
| -- | -- | -- | -- |
| R | +0 | -1 | +1|
| P | +1 |+0 | -1|
|S | -1| +1| +0|


Let’s re-frame this a little bit, by calling r, p and s probabilities that the opponent will make each respective throw. For example, suppose you know ahead of time that your opponent is using a strategy of r=0.5, p=s=0.25 (that is, they throw 2 rock for every paper or scissors). What’s the best counter-strategy?

To answer that question, we can construct a set of three equations that tells you your payoffs for each throw:

|Payoffs|
|---|
|R = 0r + (-1)p + 1s = s-p|
|P = 1r + 0p + (-1)s = r-s|
|S = (-1)r + 1p + 0s = p-r|


So based on the probabilities, you can calculate the payoffs. In the case of our rock-heavy opponent, the payoffs are:
* R=0
* P=0.25
* S=-0.25

Since P has the best payoff of all three throws, assuming the opponent doesn’t vary their strategy at all, our best counter-strategy is to throw Paper every time, and we expect that we will gain 0.25 per throw – that is, out of every four throws, we’ll win one more game than we lose. In fact, we’ll find that if our opponent merely throws rock the tiniest, slightest bit more often than the others, the net payoff for P will be better than the others, and our best strategy is still to throw Paper 100% of the time, until our opponent modifies their strategy. This is significant; it tells us that an intransitive mechanic is very fragile, and that even a slight imbalance on the player’s part can lead to a completely dominant strategy on the part of the opponent.

Of course, against a human opponent who notices we’re always throwing P, their counter-strategy would be to throw a greater proportion of s, which then forces us to throw some R, which then causes them to throw p, which makes us throw S, which makes them throw r, and around and around we go. 

# Economy
Every RTS game has an internal economy in form of resourse gathering and managing. The first step for creating a game economy system is to determine every resource type that the worker units will be able to gather in the game. When I talk about worker units, I’m talking about the units whose function is not to battle, but to gather resources and construct buildings. 

It is important to say that as less resource types a game has the more easy will be to balance the game economy.

To calculate this index and to start determining how the economic system of the game will work, first it will have to be determined how many resource units there will be in a sample stage of the game, and how many resource every resource type will have.

As an example, let’s say we have 22.398 units of resource in a sample map;

12.352 of these units of resource will be gold
10.046 will be lumber
We have more gold than lumber, so gold as being more common than lumber will have a rarity index of 1. To calculate the rarity index, we’ll need to divide the two resources by the total quantity of resources.

gold/resources ≈ 0,55 lumber/resources ≈ 0,45

After having done these calculations, to obtain the rarity index we will just subtract the result of the most common resource with the one that we want to obtain the index from, and then add 1 to the result. So in this case we would have:

rar. indx. lumber = 0,54 - 0,45 + 1 = 1,1

So after having this, we can extrapollate the rarity index formula. The common resource will be called A, the uncommon resource will be called B and the total number of resources will be called R:

rar. indx. = A/R - B/R + 1

With this rarity index we will be able to calculate the total cost of anything we want to calculate the cost from, being buildings, units or upgrades; with this formula:

cost(n) = a * aRI + b * bRI + … + (n-1) * (n-1)RI + n * nRI

This formula takes in account a number of resources n. a,b,c… are the resource quantity; the resource with the RI are the rarity index for each resource, and n is the last resource of every resource the player can dispose of, being n-1 the resource that comes before n.

For conceptualizing a game economy system, we could also do the opposite from this, in other words, the desingers of the game could determine the number the resources the game has and its rarity, and calculate the number of resource units every stage should have.

To let everything clear, when conceptualizing a level, using this rarity index to balance out how every resource will be distributed is extremelly useful, but it doesn’t need to be 100% extremelly accurate, because as I explained before, a little bit of unbalance can have positive results in the overall experiecne of the player.

Build rate
This game economy that has to be set up in an RTS game has a very clear function, that’s the one of allowing the player to progressively build their army. As I said in the last section, this system needs a coherence in its balancing, because an RTS game with a bad sense of progrssion would greatly injure one of the two big parts of these types of games, that is the part of having to strategize a good way of managing your base to allow for a fast army construction.

When utilizing a game economy system to determine the construction of a base and an army in the game, we have two parameters to take into account: the cost of each element, and how many time to build in seconds would each element dispose of. In this section I’ll be focusing on how to have a nice and balanced build rate for the elements of an RTS game, respecting their cost.

Before diving right into the calculations, it should be noted that as a rule of thumb, buildings should take more time and resources to build than unit upgrades, and unit upgrades should take more time and resources than units; because of permanency and significance in the overall game. In other words, buildings are more important than the other two elements for allowing the creation of these two, and unit upgrades are more important that units, for being permanent and having more importance overall through the course of a level.



To make a balanced build rate, first we’ll need to make sure that we have a base cost and build time for a base component of the game. Let’s say we found an adequate cost for a unit through the methods I’ve displayed in one of the first sections of this research project. Having this base cost, we will determine a base time of production for this element. If this element (it can be anything: a building, unit, unit upgrade) has a small cost, it shoud take a short time to be produced, and if it has a big cost, it would need more time of production. We want these base parameters to determine a number that will be important in the formula we’ll be using to balance out all the build rate of the game. Let’s call this parameter time adaptor. To find this parameter we’ll need to apply this formula to the set of parameters we already have (TA is the time adaptor, and every other parameter is explained in the previous section):

TA(n) = (a * aRI + b * bRI + … + n) * nRI/build time

Taking the formula to calculate a general cost of an element of the game, that I explained in the last section, we can dramatically simplify this equation to:

TA = cost/build time

Putting an example of this formula, we have a base unit that costs 300 gold (common resource), doesn’t need any uncommon resource to be created, and takes 10 second to build:

10 = 300 * 1 / X -> X = 30

The unit set of this game would have a time adaptor of 30.

After having this parameter defined, we can now apply the formula that will allow us to have a progressive build rate depending on the cost every element of the game has:

build time(n) = (a * aRI + b * bRI + … + n * nRI) / TA

Again, taking into account the formula of the last section of this document:

build time = cost/TA

As an example, I’ll will assume the base unit on which I did calculations before is a peon; and with this I will create more elements for the game and apply the build time formula to them. In this theoretical set of elements, my common resource will be gold, and my uncommon resource, with a rarity index of 1.3 will be lumber. I will round up decimal numbers, for the sake of clarity.

Gold	Lumber	Build time (s)
Peon	300	0	10
House	700	500	45
Peon Upgrade	400	100	18
Flat	1200	700	70
With this table, it can be observed that every build time has a small progressive scalation depending on the resources it uses, so it can be determinded that this method is useful for a progressive, steady scalation of the game elements of an RTS; more than a one with a slow start but fast paced rhythm at later stages of the game. Depending on the game, if you wanted to make it resource heavy, or really slow paced, you would need to change the base elements to have a bigger or smaller gap bettween the cost and build time. It would be recomended, that more than making one big table for every element of the game, a table for every element type (buildings, unit upgrades, units, etc) would be done, having each element type their own build rate scalation, and not having only one in the entire game; in this way, it would be easier to balance every element of the game.
- Tech Tree
- Maps
- AI
