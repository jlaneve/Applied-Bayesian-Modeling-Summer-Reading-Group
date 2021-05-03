# Applied-Bayesian-Modeling-Summer-Reading-Group

### Sign-up link here!

## FAQ

### What is this?

This is the landing page for an introductory-level student-run reading group on Bayesian modeling, which will held during June and July of 2021. The purpose of this group is to bring together a group of students interested in learning about Bayesian methods who might not encounter them otherwise, and have a bit of fun while doing so. This group will be application-driven rather than theory-focused, meaning that we will be more concerned with learning how to apply Bayesian methods and software tools to real-world problems than with discussing all of the intricate mathematical details. While this is a "reading" group, we will be running quite a bit of code since this material is best learned by running the examples yourself.

Our reading material will consist of a blend of books, Jupyter Notebooks, blog posts, and software documentation pages. To get an idea of some of the material we will cover, check out Richard McElreath's [Statistical Rethinking](http://xcelab.net/rm/statistical-rethinking/) and Cameron Davidson-Pilon's [Bayesian Methods for Hackers](https://github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers). In terms of software, we will be using the popular Python library [PyMC](https://docs.pymc.io/) for our computational examples but might also discuss some of the other tools that are out there.

### What are some examples of what I'll learn to do?

An excellent set of examples of Bayesian models can be found in the [examples section of the PyMC documentation](https://docs.pymc.io/nb_examples/index.html) (this is what we'll be using to implement models). On a very high-level, suppose you have some data observations and a statistical model for what you think generates your data. Your model will depend on various parameters (e.g. if the data is linear, you would have a parameter for the slope, the intercept, and possibly the variance of the observational noise). Bayesian inference answers the question: given my model and my prior beliefs about the parameter values, what are the most likely values for each of my model parameters conditional on my observed data?

Here's a quick example. Suppose you observe a series of observations along a sample path of a [geometric Brownian motion](https://en.wikipedia.org/wiki/Geometric_Brownian_motion) (don't worry if you don't know what this is!), such as shown below.

<img src="https://qed404.com/static/assets/gbm_path.jpg"/>

The geometric Brownian motion model depends on two parameters, namely mu and sigma. So, given our data observations above, what can we say about the values of mu and sigma? After we place some prior distribution on these parameters, we can use Bayesian inference to get a sense of what the most likely values for mu and sigma are.

<img src="https://qed404.com/static/assets/gbm_trace.jpg"/>

The histograms above indicate our posterior distributions over these two parameters given our model, prior, and data. An interesting thing to note about Bayesian models is that they are [generative](https://en.wikipedia.org/wiki/Generative_model), meaning that it is straightforward to then generate "fake" data that mimics our data observations, which very well could've been the data we observed should randomness have played out differently.

<img src="https://qed404.com/static/assets/gbm_post_pred.jpg"/>

Still not sure if you're interested? Checkout some recordings of the talks that were given at [PyMCon 2020](https://pymc-devs.github.io/pymcon/schedule) or [this podcast](https://www.learnbayesstats.com/) on Bayesian statistics for some more examples.

### Why is this?

Many students don't typically encounter Bayesian methods in their coursework, and even if they do they often are just introduced to the basic theory rather than how to go about building models themselves. Bayesian modeling can be a bit challenging to get started with on your own, and this group is meant to equip beginners with what they need to know in order to pursue whatever projects or applications they might be interested in.


### Who is this?

This group will be led by Jonathan Lindbloom (myself) and Julian LaNeve; participants will largely be students from our own SMU academic bubbles but we are open to others who are interested. We are shooting for a group of about 10 people.


### When/where is this?

We will meet (virtually) one evening per week (day TBD) for approximately 1.5 hours to discuss the reading for each week and some computational examples. We will begin each meeting with a brief synopsis of the material to make sure everyone gets the gist of what was covered, and then open the floor for discussion. Participants are encouraged to spend time outside of the meetings and readings playing around with code themselves, and technical support / office hours will be available to help.


### Target Audience?

In order to get the most out of this group, participants should have some prior programming experience (not necessarily Python) and at least an introductory probability/statistics class. Asides from that, this group is really aimed at people who are complete beginners to Bayesian statistics so not much else background is necessary.


### Projects?

Participants will be highly encouraged to plan and conduct their own original project to complete alongside the reading group. Guidelines for this are open-ended and participants can make their projects as involved as they would like - you'll get out of the project what you put into it. Jonathan will be available to meet and help you out with planning/implmenting your project if desired. Depending on how the projects turn out, we may try to assemble them all into a notebook or a report. 


## Outline

This is a very rough outline of what we'll cover each week. SR stands for the Statistical Rethinking book, BMH stands for the Bayesian Methods for Hackers book.

| Week | Topic                   | Readings             | Examples |
|------|-------------------------|----------------------|----------|
|  #1  | **Introduction.** Bayesian vs. Frequentist, weighted coin-flipping, Bayesian linear regression, hypothesis testing.            | SR Ch. 1; BMH Ch. 1           | None |
|  #2  | **Ingredients for a Model.**  | TBA                  | TBA      |
|  #3  | TBA                     | TBA                  | TBA      |
|  #4  | TBA                     | TBA                  | TBA      |
|  #5  | TBA                     | TBA                  | TBA      |
|  #6  | TBA                     | TBA                  | TBA      |
|  #7  | TBA                     | TBA                  | TBA      |
|  #8  | TBA                     | TBA                  | TBA      |
