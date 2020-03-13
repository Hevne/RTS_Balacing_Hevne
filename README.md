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

To create a well balanced game economy system we will have to take in account 5 steps:

* Step 1:Determine basic game values and quantify them

* Define investment and non-investment resources
* Build a cost system
* Create deficit and surplus
* Decomposition
- Tech Tree
- Maps
- AI
