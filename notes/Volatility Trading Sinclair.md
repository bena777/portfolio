### By Euan Sinclair 
#Quant_Finance 
## Thoughts
Pretty solid book that intuitively explains some options related stuff. I already knew most of the content in this book at least on the surface level but it allowed me to deepen that knowledge and see it from a new perspective such as his extremely intuitive derivation of the BSM formula. Loved the start of the book a lot more as there was not a lot of pure math and just basically intuition about the markets in general which I always prefer. However, the hedging chapters (4+5) I just simply did not understand due to the complexity of the math which is why there are no notes for that chapter. 

## Notes:
### Chapter 1: Option Pricing

"The BSM formalism becomes the conceptual framework for an options trader: In the same way that we hear our own thoughts in English, an experienced derivatives trader thinks in the BSM language." (7)

"implied volatility is the wrong number we put into the wrong formula to get the correct option price" (13)

### Chapter 2: Volatility Measurement/Forecasting

"It isn’t just the forecast that is necessary. It is putting the forecast into the context of a volatility range" (39)

### Chapter 3: Implied Vol Dynamics

"The dynamics of the smile can be seductive, and a lot of very smart people have spent a lot of time and money examining its dynamics, but the level of volatility is many times more changeable and hence more economically significant" (47)
	- The dynamics of the IV smile are not as important as I may of thought. I have spent a lot of time looking for irregularities on the actual surface itself like when I noticed AMC OTM IV was lower than ATM IV but Sinclair says that the overall LEVEL is way more important which I kind of knew but was surprised he disregarded the shape of the surface since I thought both were important


$σ12= \sqrt{σ_2^2T_2−σ^2_1T_1}$
###### The amount of volatility implied between the expirations
where 
	σ 1 is the implied volatility of the front month
	σ 2 is the implied volatility of the second month

$\sigma e = \sqrt{T_1(σ_1 ^2 - σ_{12} ^2)}$
$E = \sqrt{\frac{2}{\pi}}*σe$
##### This equation is used to find the absolute expected jump

"Even if all the components have flat implied volatility surface, the index can exhibit a smile if correlation is expected to increase as the underlying moves." (55)

### Chapter 6: Money Management

* *"Everybody's got a plan until they get hit" - Mike Tyson

* Certain elementary strategies such as doing what you "feel like" or setting a fixed amount to each trade are used but do not work the best

* Trade bigger when there is more edge, smaller when there is less
* It is a bad idea to add stuff like stop losses to a trade
* Trade big enough that the profits actually mean something but not SO big that the losses would be a significant part of your portfolio


* Overall, far and away the best strategy to use is the famous [[Kelly Criterion]]

##### Alternatives to the Kelly:
- Oscar's System- the infamous system of "doubling down overtime you lose"
	- Negative progression: raising bets as you lose more 
	- Can work better than Kelly in some place but when it goes bad it is terrible
	- _Example_: I bet $10 on a coin flip where the betting limit is $100. If I lose 4 times in a row which is unlikely but possible, I am kind of fucked and the system goes to shambles 
* Browne's System
	- Maximizes the probability of reaching a SET level of wealth in a certain amount of time 
	- Can be useful when dealing with a fixed goal 
	- Is used in the derivative markets often 


### Chapter 7: Trade Evaluation

* "In theory there is no difference between theory and practice. In practice there is" - Yogi Berra (127)

- Tracking the results of a trade is extremely important; I feel I do this in my brain already but it could definitely make sense to put it down on paper or Excel sheet
- One idea I had for this to solve the issue of depositing money is to start at a set number of $10,000 and just multiply that number by my percentage returns each day to gain an accurate refection of my performance 

* A lot of the methods in this chapter are more for the industrial trader rather than retail so I probably won't be using them 

#### Risk Metrics

* Sharpe Ratio- the most common and simple risk adjusted return metric 
	- Simply the excess risk free return divided by volatility
	 $$ SR=\frac{\mu-r}{\sigma} $$
	 * Simple and effective method of risk adjusted returns
	 * The main issue is that it is based on historical volatility; we have know way of knowing if this is implicative of future realized vol 
	 * It seems easy to "game" as the author put it, selling OTM options can easily have a high Sharpe ratio since the huge event that is priced in HAS NOT HAPPENED YET. This is probably why [[Nassim Taleb]] is not a fan of any of these metrics. 
* Sortino Ratio- same as Sharpe except it is only DOWNSIDE volatility instead of either side
$$ Sortino = \frac{\mu-r}{\sigma_d}$$
* Calmar Ratio- same as two above except it uses maximum drawdown
*$$ Calmar = \frac{\mu-r}{drawdown}$$
* Continue to do a trade if the personal view has not changed, this should not change based on simply having 2-3 down days in a row but should instead be if something FUNDAMENTAL such as the vol prediction in a trade has changed
* Even a good +EV strategy can go through bad periods due to the basic laws of probability
### Chapter 8/9: Trading Psychology
* "Man uses psychology exactly like his ancestors used witchcraft; anything you don't understand, it's psychology- Bill James" (149)
* "We must remember that winning trades are typically dependent on a large number of factors, with luck being the largest component of any individual trade" (152)
* "Humans don't have a systemic tendency toward either under or overreaction. They have a tendency toward mis reaction" (160)
* "Be aggressive in looking for evidence that contradicts your view or position" (163)