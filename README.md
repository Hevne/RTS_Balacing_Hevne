# Introduction


# Intransitive Mechanics or Rock Paper Scissors (RPS)

Intransitive Mechanics is just a geeky way of saying "Rock-Paper-Scissors like game" these are the games which don't have a single dominant strategy, because everything is weak and strong at the same time against something else, a kind of zer-sum games.

We see intransitive mechanics in games all the time. In fighting games, a typical pattern is that normal attacks are defeated by blocks, blocks are defeated by throws, and throws are defeated by attacks. In real-time strategy games, a typical pattern is that you have fliers that can destroy infantry, infantry that works well against archers, and archers are great at bringing down fliers.

Some of these relationships might not be immediately obvious. For example, consider a game where one kind of unit has long-range attacks, which is defeated by a short-range attacker who can turn invisible; this in turn is defeated by a medium-range attacker with radar that reveals invisible units; and the medium-range attacker is of course weak against the long-range attacker.

![](https://github.com/Hevne/RTS_Balacing_Hevne/blob/master/rps.png)

## Why Intransitive Mechanics?

It may be worth asking, if all intransitive mechanics are just glorified versions of Rock-Paper-Scissors, what’s the appeal? Few people play Rock-Paper-Scissors for fun, so why should they enjoy a game that just uses the same mechanics and dresses them differently?

For one thing, an intransitive game is at least more interesting than one with a single dominant strategy (“Rock-Rock-Rock”) because you will see more variety in play. For another, an intransitive mechanic embedded in a larger game may still allow players to change or modify their strategies in mid-game. Players may make certain choices in light of what they observe other players doing now (in real-time), particularly in action-based games where you must react to your opponent’s reaction to your reaction to their action in the space of a few milliseconds.

Additionally, intransitive mechanics serve as a kind of “emergency brake” on runaway dominant strategies. Even if you don’t know exactly what the best strategy in your game is, if all strategies have an intransitive relationship, you can at least know that there will not be a single dominant strategy that invalidates all of the others, because it will be weak against at least one other counter-strategy. 

Intransitive mechanics can be tangled as much as the designer wants to but its better to keep it simple for the player having the classic formula of a relation between 3 used in games as Pokemon, Starcraft, Civilization or even Dark Souls. Just imagine playing a game and having to take in account all these relations:

![](https://retrohelix.com/en/wp-content/uploads/2013/08/rps11.jpg)

# Some Maths behind RPS games

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

Since P has the best payoff of all three throws, assuming the opponent doesn’t vary their strategy at all, our best counter-strategy is to throw Paper every time, and we expect that we will gain 0.25 per throw – that is, out of every four throws, we’ll win one more game than we lose. 

In fact, we’ll find that if our opponent merely throws rock the tiniest, slightest bit more often than the others, the net payoff for P will be better than the others, and our best strategy is still to throw Paper 100% of the time, until our opponent modifies their strategy. This is significant; it tells us that an intransitive mechanic is very fragile, and that even a slight imbalance on the player’s part can lead to a completely dominant strategy on the part of the opponent.

Of course, against a human opponent who notices we’re always throwing P, their counter-strategy would be to throw a greater proportion of s, which then forces us to throw some R, which then causes them to throw p, which makes us throw S, which makes them throw r, and around and around we go. 

# Tactics taken in account on an RTS
How much strategy is needed in an RTS to win a human opponent? Assuming that RTSs can be simplified to the Rock-Paper-Scissors (RPS) formula makes this last question a lot easier to answer since a chinese university has found the always-winning strategy for an RPS based game.

Is stated that if a player wins over her opponent in one play, her probability of repeating the same action in the next play is considerably higher than her probabilities of shifting actions. If a player has lost two or more times, she is likely to shift her play, and more likely to shift to the play that will beat the one that has just beaten her than the same one her opponent just used to beat her.

So its clear that if a player takes in account this method when confronting another player he has a significantly higher rate of winning since he can constantly predict the movements or strategy that will follow the other player in order to beat him.

If I'm Alex and my rival is Paul, Paul has been trying to destroy my tanks using infantry units and by now his troops has been oblittered so he is more likely to start producig anti-tank troops, knowing this I can anticipate and prepare infantry units to counter his anti-tank troops.

![](https://qph.fs.quoracdn.net/main-qimg-5f2c081d0d447b96b6fc74a2bb71ae98.webp) 

But as I stated before: two conscious and gamer players can be engaged on a constant loop if following this strategy so, how to solve this situation?

# Solving the human opponent problem

Rock-Paper-Scissors is a symmetric zero-sum game, so:

**R = P = S = 0**

Since the opponent must select exactly one throw, we also know the probabilities of their throw add up to 100%:

**r + p + s = 1**

From here we can solve the system of equations by substitution:

* **R = 0 = s-p** therefore p=s
* **P = 0 = r-s** therefore r=s
* **S = 0 = p-r** therefore p=r
* **r+p+s = r+r+r = 1** therefore r=1/3 
* **Since r=p=s** therefore p=1/3, s=1/3<br>

So our solution is that the opponent should throw r, p and s each with probabilities of 1/3. This suggests that against a completely random opponent it doesn’t matter what we choose, our odds of winning are the same no matter what. Of course, the opponent knows this too, so if we choose an unbalanced strategy they can alter their throw ratio to beat us; our best strategy is also to choose each throw with 1/3 probability.

Note that in actual play, this does not mean that the best strategy is to actually play randomly (say, by rolling a die secretly before each throw)! As I’ve said before, when humans try to play randomly, they tend to not do a very good job of it, so in the real world the best strategy is still to play each throw about as often as any other, but at the same time which throw you choose depends on your ability to detect and exploit patterns in your opponent’s play, while at the same time masking any apparent patterns in your own play. So our solution of 1:1:1 does not say which throw you must choose at any given time (that is in fact where the skill of the game comes in), but just that over time we expect the optimal strategy to be a 1:1:1 ratio (because any deviation from that hands your opponent a strategy that wins more often over you until you readjust your strategy back to 1:1:1).

# Bibliography
* [The Balance of Power: Progression and Equilibrium in Real-Time Strategy Games](https://www.gamasutra.com/blogs/BrandonCasteel/20170306/292982/The_Balance_of_Power_Progression_and_Equilibrium_in_RealTime_StrategyGames.php)
* [Intransitive Mechanics](https://gamebalanceconcepts.wordpress.com/2010/09/01/level-9-intransitive-mechanics/)
* [Examining the Implementation of Rock, Paper, Scissors, Balance in Video Games](https://www.youtube.com/watch?v=N69Jzzcu57Q)
* [Perfect Imbalance](https://www.youtube.com/watch?v=e31OSVZF77w)
* [Applying RPS to games](https://www.gamasutra.com/blogs/DevonWiersma/20170428/297030/Applying_Rock_Paper_Scissors_to_Video_Games.php)
* 
