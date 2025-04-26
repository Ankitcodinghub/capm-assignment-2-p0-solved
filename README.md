# capm-assignment-2-p0-solved
**TO GET THIS SOLUTION VISIT:** [CAPM Assignment 2 P0 Solved](https://www.ankitcodinghub.com/product/capm-p0-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;124873&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CAPM Assignment 2 P0 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
wrap: sentence

—

“`{r setup, include=FALSE} knitr::opts_chunk$set(echo

= TRUE)

“`

No discussion with a fellow student is allowed.

Use the getfinmdat() function in the cbw library to download monthly excess returns on apple (ticker symbo

Call the downloaded object datdf.

Use the data in datdf for Questions 1-3.

## Question 1

Suppose you are interested in estimating the CAPM model $$

ext{prmapple} = eta , ext{prmsp500} + e

$$ where you assume that $e$ is N(0,$sigma^2$).

Assuming that the data you have downloaded can be thought of as a random sample, answer the following

1. What is the dim of datdf?

2. Write a function dnormal that takes as inputs a vector y, mean vector mu and variance parameter sigma The parameter sigma2 is common to each of these densities.

3. Use the dnormal function to write down a function to calculate the loglikelihood function of theta = (beta,

This is the sum of the log of the month-by-month normal densities of prmapple given prmsp500 and the p

The log-likelihood function should take two inputs, theta and datdf, and return the log of the likelihood fun

4. Write down another function that calculates the cost function of theta = (beta,sigma) (this is the negative

5. Use the ucminf function to minimize the cost function over theta = (beta,sigma).

Call this minimizing value thetahat = (betahat,sigmahat).

Use (1,.03) as the starting values.

Ask the ucminf function to output the hessian.

6. Use the cbind function to put thetahat and the standard errors of thetahat in a matrix object.

The se is the sqrt of the diag of the inverse of the hessian.

“`{r}

# write your code here

“`

## Question 2

Suppose you estimate the CAPM model in Question 1 by Bayesian methods.

The difference now is that we treat the parameters theta = (beta,sigma2) as random variables. We put a prior on theta and combine the prior with the likelihood by Bayes theorem to get the posterior dist Use the MCMCregressg function in the cbw package to answer the following questions.

1.

Do a Bayesian estimation of the CAPM model with the data in datdf.

Make sure when you specify the model formula that there is no intercept in the model.

Use the default 15% of the data to form the training sample prior.

2.

What are the posterior mean, sd and the .025 quantiles of beta from this Bayesian estimation?

3.

Is the posterior mean of beta similar to the estimate of beta you got by minimizing the cost function?

Is the posterior sd of beta similar to the se of betahat in Question 1?

4.

The MCMCregressg output sends out draws of sigma2 from the posterior distribution.

Use these draws to calculate the posterior distribution of sigma.

What are the posterior mean, sd and .025 and .975 quantiles of sigma?

How do these compare with the sigmahat and se of sigmahat you got in Question 1?

“`{r}

# write your code here

“`

## Question 3

1. Instead of using a training sample prior, suppose you specify your prior on the parameters. Suppose tha

“`{r}

# write your code here

“`
