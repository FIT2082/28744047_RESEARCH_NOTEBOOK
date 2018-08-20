# Week 4 Progress

## *Meeting*
This week's meeting was mostly centred around discussing our Project Specification, the new data obtained, as well as 
future methods to analyse the data. The new data provided by Monash building managers is Chiller data consisting of temperature levels,
past alarms, demand response and many more relevant variables. Upon brief inspection of the data, the alarm data provides the most information
as it describes what fault occurred and when and where it occurred. This allows us to determine problematic areas of plants and can give us
insight into possible trends reflective of the data. The only challenge we face with this is that there is an insufficient
amount of data to formulate a noticeable pattern, therefore the best approach to getting somewhere is to cross check the faults with
the different variables (eg. temperature, etc.) to be able to make correlations of significance.

## *Plots*
After the meeting, Andrew offered to make plots for each of the variables so that we could begin our initial analysis of the data.
The plots have been generated in R and demonstrate a year's worth of trends for a specific variable, which make it easier to isolate 
problematic factors and cross check the alarm faults with the relevant variables. Below is an example of a plot that raises some concerns:


<p align="center">
<img src="https://github.com/FIT2082/28744047_RESEARCH_NOTEBOOK/blob/master/Week4plot.png" width="500" height="400" />
</p>


Why is there a sudden spike around early March? This variable may be affecting other variables such as Chilled Water Return Temperature
to encounter similar issues, which may lead to a bigger problem later on. Based on these plots, we can further investigate such
"problem" variables and thus ascertain what indeed can contribute to overall plant failure.

## *Plan of Action for Week 5*
* Analyse generated plots.
* Explore trends and find meaning in the data.
