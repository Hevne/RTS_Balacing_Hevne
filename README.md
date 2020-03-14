# Introduction
My name is Eudald Garrofe, I'm a student from CITM's videogames design & development degree. On this website I'm going to explain my research on RTS Balancing focusing on Rock Paper Scissors base.

# Index
* <a href="#Intransitive Mechanics or Rock Paper Scissors"><b> 1. Intransitive Mechanics or Rock Paper Scissors</b></a>
* <a href="#Why Intransitive Mechanics?"><b> 1.2. Why Intransitive Mechanics?</b></a>
* <a href="#Some Maths behind RPS games"><b> 2. Some Maths behind RPS games</b></a>
* <a href="#Tactics taken in account on an RTS"><b> 3. Tactics taken in account on an RTS</b></a>
* <a href="#Solving the human opponent problem"><b> 4. Solving the human opponent problem</b></a>
* <a href="#Bibliography"><b> 5. Bibliography</b></a>


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
|R = 0r + (-1)p + 1s = s-p|
|P = 1r + 0p + (-1)s = r-s|
|S = (-1)r + 1p + 0s = p-r|


So based on the probabilities, you can calculate the payoffs. In the case of our rock-heavy opponent, the payoffs are:
* R=0
* P=0.25
* S=-0.25

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

**R = P = S = 0**

Since the opponent must select exactly one throw, we also know the probabilities of their throw add up to 100%:

**r + p + s = 1**

From here we can solve the system of linear equations by substitution:

* **R = 0 = s-p**   therefore p=s
* **P = 0 = r-s**   therefore r=s
* **S = 0 = p-r**   therefore p=r
* **r+p+s = r+r+r = 1**   therefore r=1/3 
* **Since r=p=s**   therefore p=1/3, s=1/3<br>

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

