
# The Poisson Distribution
The poisson distribution has a special relation to the binomial distribution. The theoretical underpinnings are as follows. Imagine that we take a time period and break it into subintervals that are so small that at most one successful event could occur. We can then imagine that for any of these subintervals, a binomial distribution could apply where there is some probability of the event occuring p, a probability q=1-p that the event does not occur, and a probability of 0 that more then one event occurs. We assume that as we cut time into smaller and smaller intervals, the chance of a success should go down. If we take the limit of the binomial distribution as n goes to infinity (more and more subintervals that are progressively smaller), the result is the poisson distribution.

Binomial Probability Distribution:  
$p(y) = \binom{n}{y}p^y(1-p)^{n-y}$
  
$\lambda = n*p$  
  
Poisson Probability Distribution:
$p(y) = \frac{\lambda^y}{y!}e^{-y}$
  
  
Also note that labmda is the now the average number of successes that we anticipate in a given interval. (The probability p of success, times n the number of intervals.) This is then exactly how the poisson is used in practice, if I know the average number of occurences in a given interval, what is the probability that the actual number of occurences is slightly more, slightly less, far more or far less?

# Poisson Function
Write a function to calculate the probability that y events occur in a given interval given the average number of occurrences expected.


```python
def poisson(y, mu):
    #Your code here
    return prob
```

# Reinventing the Wheel
Check that your poisson function above works by checking its output for 1000 examples against scipys built in function:  
scipy.stats.distributions.poisson.pmf


```python
#Your code here
```

# Mail
Let's say on average, you receive 4 pieces of mail per day. Draw a graph with the x-axis pieces of mail (0-20) and the y-axis the probabilitiy that you receive that many pieces of mail on a given day.


```python
#Your code here
```

# Home Runs
https://www.teamrankings.com/mlb/stat/home-runs-per-game  
  
On average, the Yankees hit 1.47 home runs per game in 2017. What was the probability that they hit 2 home runs in a game? 3?


```python
#Your code/answer here
```

# Home Runs 2
In the same year, the Red Sox only had 1.04 home runs per game in 2017. What was the probability that they hit 2 home runs in a game? 3?


```python
#Your code/answer here
```

# Product Failures
Airplane tires need replacement after about 1500 flights. Let's assume that on an average day, an airline has to replace 2.34 tires per day. If you want to have a 95% confidence that you'll have enough tires for needed repairs, how many should be on stock? (We want to have enough, but storing tires is also expensive!)


```python
#Your code/answer here
```

# Product Failures 2
How many tires do you need on stock to have a 99% confidence that you'll have enough in stock? 99.9% confidence?


```python
#Your code/answer here
```
