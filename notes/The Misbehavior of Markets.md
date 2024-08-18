## By Benoit Mandelbrot


# Summery:

An enjoyable and  intuitive read that provides a glimpse into many unique concepts in a short span. I do wish that he dove SLIGHTLY more into the theory in the book but I do see that its a very fine line to go from an entertaining philosophical commentary of the markets to a straight up boring math textbook like so many of these types of books do. Allowed me to explore concepts such as [[Modern Portfolio Theory]], [[Fractal Geometry]], and [[Power Laws]] in detail. Definitely one of my personal favorite books about the market I've ever read and Mandelbrot comes off as a less bold, kinder, and more accepting version of [[Nassim Taleb]]. I look forward to exploring the concepts laid out in this book in more depth over the next few months.


#Quant_Finance 
# Annotations:

## Chapter 1: Risk, Ruin and Reward

* ##### This chapter sets up a strong introduction to the book by going over the idea that we are not properly prepared for risks in the financials markets. He criticizes both the efficient market theory as well as the idea that price changes are normally distributed. The influence on [[Nassim Taleb]] is extremely clear. He also shits on technical analysis which is always nice. 

*  "In the fun-house mirror logic of markets, the chartists can at times be correct. Stock quotes really can approach a level advertised by chartists, and then pull back as if hitting a solid wall- or accelerate as if bursting through a barrier. But this is a confidence trick: Everybody knows that everybody else knows about the support points, so they place their bets accordingly" (9)
	* Brilliant explanation of how TA works and while he mainly shits on it, it shows how it can work in certain situations 
* "Price changes are not independent of each other" (11)
	* Yesterday and the day before price DOES influence the next day
	* Curious to see what this "long memory" concept of his is 
	* While he doesn't use the terms I'm used to, it is clear that he is saying that volatility tends to cluster which is sometime I had established a long time ago


## Chapter 2: By the Toss of a Coin or the Flight of an Arrow

*  Mandelbrot goes into the concept of chance here and how it can have many different definitions
* ##### The market do not just move by chance. Market movement SEEM to move by chance to us but this is not the case 
	* "That subtle distinction, of thinking about prices as if they were governed by chance, has been the dominant, fructifying notion of financial theory for the past one hundred years" (26)
	* If we were suddenly given God like powers and were able to see every single event happening on the world at once, we could theoretically predict stock prices. However, this is extremely impractical for obvious reasons which leads us to the black box approach of using probability as our best tool since we don't know what is happening during the process to produce the outputs it does . This concept can be applied to other fields as well such as physics.
	* "But to say the record of transactions, the price chart, can be described by random processes is not to say the chart is irrational; rather, it is to say it is unpredictable" (29)
#### Types of randomness:

#### Mild-
* The classic Gaussian distribution that can be used to describe many natural processes such as average IQ or height 
#### Wild-
* The "fat tailed" distribution described by [[Nassim Taleb]]
* Cauchy was one of the first to bring this to light 
* Non normally distributed errors with both infinite mean and variance; it is safe to say that process that have Black Swan type events follow this type of randomness

## Chapter 3: Bachelier and His Legacy

* ##### A history based chapter that shows the life of Louis Bachelier and how he set up the foundations of modern financial theory 

* "A scientist worth of the name, above all a mathematician, experiences in his work the same impression as an artist; the pleasure is as great and of the same nature" (44)
	* Literally what I was thinking about last night when I heard about Camus talking about how art provides people with a deep satisfaction 


## Chapter 4: The House of Modern Finance

* ##### An interesting layout of a chapter with even more history setting the stage for the "house of cards" of modern finance which he later deconstructs throughout the rest of the book

* "A portfolio is efficient if it produced the most profit with the least amount of risk" (65)
* ##### Markowitz-
	* Invented the idea of [[Modern Portfolio Theory]]
	* Strong proponent of diversity; combine a bunch of stocks with opposite betas 
	* The issues with his model is that it requires a LOT of prediction most of which relying on historical data which is not always the best tool for every situation 
* ##### Sharpe- 
	* Invented the famous share ratio: 
		 $$s_a=\frac{R_a-R_f}{\sigma_a}$$
		Where $R_a=$ Asset return and $R_f= $risk free rate
	* Invented the [[CAPM]] model
* I love that this book reads like a novel even though its nonfiction; Mandelbrot is building up the house of cards that is modern portfolio theory even giving the history of those that created it only to bring it down in the coming chapters (hopefully)

## Chapter 5: The Case Against Modern Financial Theory

* ##### A short chapter that discusses the vast assumptions that modern financial theory makes; honestly wish this chapter was a bit longer

* ### People are rational:
	* People react differently to news about stocks; some are more risk adverse than others as well as having different timeframe
* ### Price changes are continuous 
	* This is obviously wrong since the majority of jumps happen in the beginning of each market day as well as when news comes out. Not to mention that the majority of markets are not open 24/7'
* ### Market follows Brownian Motion
	* It has been shown that the market has fats tails and does not followed a normal distribution
	* The entire financial system is built of this notion which is just flat out wrong
* "If you are going to use probability to model the financial markets, you better use the right kind of probability" (105)

## Chapter 6: Turbulent Markets: A Preview 
* ##### Introduces the concept of [[Fractal Geometry]] and how it can be applied to the financial markets

* "When we explore the vast realm of natural and human behavior, we find our most useful tools of measurement and calculation are based on surprisingly few basic ideas" (116)
* Mandelbrot goes on to show a very basic example of a fractal as shown in [[Fractal Geometry]]

## Chapter 7: Studies in Roughness: A Fractal Primer
* Dives into a deeper view of the concept of [[Fractal Geometry]] and goes on to talk about a related but different topics, dimensionality; not really related to finance at all
* "The first and oldest problems in every branch of mathematics spring from experience and are suggested by the world of external phenomena" (123)
* Fractals become both more interesting and complex as you vary the shape patterns (which can be done through randomizing patterns)
#### Dimensionality and Roughness:
* Dimension as all about perspective
	* If we see a ball of thread from far away it looks like a dot or 0 dimensional. If you hold it it goes back to our normal three dimensions. If you like at each thread individually it becomes 1 dimensional.
	* The same object can have more than one type of dimension depending opn how you look at it 
* We have a way to measure this: a measurement called fractal dimensionality
	* For a straight line, this is 1 and as areas get more and more rigid these numbers decreases and vice versa for it decreasing 
	* $$ d_s = log(N)/log(r) $$
	where:
		- $r=$ the ratio by which the shape scales up or down
		- $N=$ number of measuring units 

## Chapter 8: The Mystery of Cotton
* Describes the process in one of Mandelbrot's biggest study: the in depth study of the history of cotton prices
* Delves highly into the idea of [[Power Laws]]
*  Goes into the studies of Pareto; A man who graphed the income distribution of Italy and discovered the idea of [[Power Laws]]
* Talks about Zipf's study. One that ranks the appearances of words in a certain text.
	* The words are sorted into ranks with 1 being the most used word and so on with the formula that gives the probability of each word occurring in the text being
	* $$ Q(r)=Fr^\frac{-1}{a}$$
		where: 
			$Q=$ the probability distribution function
			$r=$ the word rank
			$F$= a constant that Zipf estimated at 1/10
			$\frac{-1}{a}=$ the power law factor
* No matter the timeframe, stock prices follow the same distribution so it can be hard to differ between daily and even minute timeframes 
	* "All look the same. A month looks like a day, one set of days like another" (164)

## Chapter 9: Long Memory: Nile to the Marketplace

* #### Introduces the concept of "long memory" and how the efficient market hypothesis fails to explain it

* "No one is alone in the world. No act is without consequences for others" (185)
* "The brain highlights what it imagines as patterns; it disregards contradictory information. Human nature yearns to see order and hierarchy in this world. It will invent it where it cannot be found" (189)

* The concept of flood prevention when building dams can be applied to some aspects of the market
* Talks a lot about the clustering of droughts/floods; similar to the proven clustering of low volatility days and high volatility days in the market 
* ##### Everything in the market is related to each other, we just don't have a way to quantify the effects (chapter 2)

* Led to the creation of the H or Hurst exponent.
	* $$ E[\frac{R(n)}{S(n)}]=Cn^H$$
	where:
		$R(n)=$ Range of standard deviations of data set
		$S(n)=$ Sum of the standard deviations of data set
		$n=$ number of observations
		$C=$ scalar constant 
	
	This H exponent measures the strength of the "long memory" of a time series; A higher H than 0.5 suggests that market movements are not independent of each other
	The H can be calculated using rescaled range analysis

## Chapter 9: Noah, Joseph, and Market Bubbles

* ##### Mandelbrot describes two distinct processes in this short chapter which culminate the previous chapters about his beliefs on how the market works 

* ### Noah Effect:
	* The "black swan" event which is compared to the flooding of the Earth in the Bible
	* Markets may be stable for a while but eventually a sudden event can happen wiping out all past gains
	* Measured using the $\alpha$ coefficient 
* ### Joseph Effect:
	* "Almost cycles"
	* There is long term memory in the market which is compared to the biblical story of Joseph selling corn to Egyptians after being shown a trend 
	* Goes along with the Hurst or H exponent
* These two effects go together, so much so that $H=\frac{1}{\alpha}$
* This is because when the market rises/falls in an "almost trend" for a while (Joseph Effect), the eventual change of direction is often both rapid and extreme (Noah Effect)
###  R/S (Rescaled-Range Statistic):
* Used to measure long-term dependence in a time series of data (which means it can be used to measure the Hurst exponent)
* Measures if over time, the amount by which the data varies from max to min is greater than if they were completely independent 

1. Calculate mean of time series dataset
2. Create a list of each change day by day
3. Calculate the mean of the list of changes
4. Create another list subtracting each change day by day from the mean of the changes
5. Using variable "r", store the max from the list in step 4 and subtract the min of it from it 
6. divide this r coefficient by the standard deviation of the original time series data 

## Chapter 10: The Multifractal Nature of Trading Time

* ##### Complicated idea piecing together all of the previous chapters in a way that I don't quite understand yet

* A multifractal is a fractal which is scaled differently in different parts; some shrink faster while some slower

* The idea of multifractal time states that in trading, when things get hot and volatility increases "time" moves faster in a sense (due to more happening in this timeframe than sometimes the rest of the day combined) and slower during less volatile periods of the day

* Mandelbrot uses this idea of multifractals to convey his idea of the [[MMAR]] or multifractal model of asset returns

## Chapter 11: 10 Heresies of Finance

1. Markets are turbulent and volatile
	* "Every event, no matter how short or long ago, echoes across all other events" (229)
2. Markets are riskier than expected
	* Due to the fat tailed distribution of the stock market, we often are taking on significantly more risk than we expect from the Gaussian distribution
3. Timings matters since volatile periods tend to cluster
	* Common idea explored about vol clustering. Periods of high volatility are more likely to be followed by more periods of high volatility and same with low 
	* Majority of gains/losses over a long period of time come over only a few days; E.G 40% of gains in the 1980s S&P was from 10 days or 0.5% of days
4. Prices are not continuous 
	* Due to binary events such as earnings or economic factors as well as markets opening and closing at specific times, we typically see jumps in prices rather than a slow glide to where it is 
5. Time is flexible
	* Different investors have different timeframes; some may be day trading while others may be swing trading over the course of a few weeks while others may be holding for a few decades
	* All chart timeframes tend to look the same due to the scalability of stock prices
6. Markets are similar in all walks of life
	* The stock market is effected by things outside of it; for example weather, macroeconomic factors, political tensions, and more
7. Markets are uncertain
	* It is basically impossible not only to predict the direction of future stock prices moves, but also the level of magnitude
8. Markets are deceptive 
	* Random noise causes us to see patterns with no statistical significance such as technical analysis 
	* It may even appear that cycles exist over time 
9. Volatility can be estimated
	* While direction is impossible to forecast, it is possible to predict volatility due to the clustering of it 
10. Value is subjective
	* Different measures of calculation lead to different values obtained 
	* At the end of the day, the true value of something is what people are collectively willing to pay for it which is essentially n,   the current trading price 