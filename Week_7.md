# Week 7 Progress

## *Meeting*
Not much has progressed in our project from the previous week, so there wasn't too much on the agenda for this week's meeting. Given that
the Monash Building Managers have still not responded to our previous email, Arnaud suggested that we should look into a Microsoft Machine
Learning tutorial that he had sent earlier and explore the tutorial to get some ideas for approaching our research problem. The tutorial is 
very much insightful and relevant to our work as it is also based on a plant failure dataset. This will be very useful to us and may help
us with our approach later on.

## *HMM Packages*
Last week I had read about Hidden Markov Models (HMM) and thought that they would be useful in our research. The following are two packages
which I believe will be useful in our project:

[HMM Package](https://cran.r-project.org/web/packages/HMM/HMM.pdf)

The HMM Package is a fairly standard library that performs the basic necessary functions required to carry out statistical analysis.
The reason why it would be good to use is that it is relatively straightforward and doesn't contain any unnecessary functions.

[depmixS4 Package](https://cran.r-project.org/web/packages/depmixS4/vignettes/depmixS4.pdf)

The depmixS4 package was created to extend the normal HMM package. The creators of the depmixS4 package state that it was created to meet 
the following goals:

1. To be able to estimate parameters subject to general linear (in)equality constraints;
2. To be able to fit transition models with covariates, i.e., to have time-dependent transition
matrices;
3. To be able to include covariates in the prior or initial state probabilities;
4. To be easily extensible, in particular, to allow users to easily add new uni- or multivariate
response distributions and new transition models, e.g., continuous time observation
models.


For the time being, I think I will practice implementing the first HMM package as it seems like a good starting point. If I feel like I need
to extend some of the functionalities, then I will consider the depmixS4 package.


## *Plan of Action for Week 8*
* Explore the Microsoft Azure Tutorial on plant datasets.
* Apply the techniques learnt from Microsoft tutorial on the existing dataset.
* Try and implement HMMs on the current dataset, although the data is not substantial.
