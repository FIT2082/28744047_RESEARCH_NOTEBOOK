# Week 6 Progress

## *Meeting*
This weeks meeting was centred around looking at the data and plots we currently have, and then brainstorming what we require further 
from the Monash Building managers. Prior to the meeting, I drafted an email that we would send to the building managers, so the meeting 
was a good opportunity to add some extra things in. Other than this, we looked at the plots generated and tried to identify trends we hadn't
looked into. For example, we were able to see that a variable that wasn't directly related to a certain fault may well indeed have caused the 
fault. This means that when we implement our predictions for different kinds of faults, we have to make sure that we consider ALL variables,
not just the relevant ones (ie. not only looking at pressure levels for differential pressure faults, etc.).

## *Literature Review*
Last week, I had set out a goal to look at relevant literature and identify the common methods applied in such journals. I found in one 
particular [article](https://www.hindawi.com/journals/mpe/2016/8705796/) that Hidden Markov Models were an ideal approach to condition-based
maintenance. Condition-Based Maintenance (CBM) is a planned maintenance that seeks to take action before a failure occurs, by inspecting
the condition of a system and predicting the likelihood of failure based on existing data. 

So what exactly are Hidden Markov Models (HMM)? HMMs are a statistical model that aims to predict a future set of states based on some 
initial states. A state denotes an event that occurs. For the purpose of understanding HMMs better, we can say that a state is whether a
variable exceeds a value that would cause a fault.

Hidden Markov Models require the following to be able to output a sequence of states:
1. *Initial state values* - The initial probabilities of states occurring. We need these initial values as they set the basis 
of determining the sequence of states.
2. *Transition matrix* - A matrix consisting of the probability of transitions from one state to another as calculated by the
Gaussian distribution. In our case this is:


| <22 degrees --> <22 degrees | <22 degrees --> >22 degrees |
|-----------------------------|-----------------------------|
| **>22 degrees --> <22 degrees** | **>22 degrees --> >22 degrees** |


3. Emission function - The emission function outputs continuous emissions, which the algorithm uses to determine what 
days exceed the normal variable levels. This is used to generate a sequence of states.


Though I have a fair understanding of HMMs, I will need to further investigate their application to this project and I should also explore
other methods that have been implemented in the past on similar research.

## *Plan of Action for Week 7*
* Explore the different predictive methods and their viability for this project.
* Read more literature relevant to the project.
