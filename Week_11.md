# Week 11 Progress

## *Meeting*
This week we had a meeting with our supervisors, Raq, one of the Monash Building Managers and someone who works at Schneider Electric. 
Initially I didn't really know what the meeting was for, but Raq elaborated on his "vision" so to speak for this project
and clarified my doubts. One of the agendas of the meeting was to ensure that everyone was on the same page and for us to properly understand the 
need for this project. We learnt that Monash University spends a lot of money on facilities, therefore being able to predict plant failure
is ideal and can save money in the long run. Raq also seemed quite keen on using mathematical techniques to find correlations between different
variables, so this is something that we should take note of to tell the next group of students that undertake this project.

Another aspect of the meeting was to give us more data. The team at Schneider Electric were happy to give us more data, which upon initial
inspection is way more complex than the Monash data. It would take some time to determine how to break up the data, so we need to decide
whether to do our testing and implementation on the Monash data and let the next group of students work with the Schneider data. If we were
early on in the semester, we could have worked with this elaborate dataset, but given that we only have one week to go, even I'd say that
it's a bit optimistic to get meaningful insights of the data.

Before the meeting, I implemented random forests on the Monash data that we recently got, so luckily I had something to show.
I calculated a Root Mean Square Error (RMSE) which is a measure of the difference between values predicted by a model or an estimator 
and the values observed. Essentially, it is a measure of accuracy, however when I ran the program I yielded a value of ~ 80.92425%. 
However, this is the first set of results that we've been able to get in this project, so while it isn't the most accurate, it most certainly
is a start.

## *Other Progress*
The main thing I worked on this week was the random forest implementation. I created a test and train set, and then used R's randomForest 
package to create the set of trees. I created 5000 trees in total so that values for each row could be calculated multiple times in order to 
maintain consistent results. I really like random forests and the "randomness" of it - this would provide more accurate results and would
avoid bias in the predictions. The only downside is that it takes a lot of time to run one command 
(eg. randomForest(HiPrssC2 ~ ., data=TrainSet, importance=TRUE, ntree=5000)). Any time I make a change, I have to run the commands again, 
which means waiting for a long time in anticipation as to whether my issue is resolved or not. Nonetheless, this is only a minor issue and 
the outcome of the results outweighs the length of the run times.

My inital plot of the error rate vs. number of trees looks like this:

<p align="center">
<img src="https://github.com/FIT2082/28744047_RESEARCH_NOTEBOOK/blob/master/week11.png" width="650" height="500" />
</p>

We can see that the more trees are generated, the lower the error rate, which further reinforces the importance of generating several trees
and calculating values for each row multiple times. While this plot looks favourable, it can definitely be improved. (Note that this plot
represents a random forest implementation on the chiller2 data that we got from Raq, hence the rf.chiller2 title)

Apart from the considerable progress this week, I've added to the final report and have also started working on the poster. We aim to have the 
poster completed by this weekend so that we enough time to get feedback and print it as well. We will also start preparing our two-minute
pitch for next week.

## *Plan of Action for Week 12*
* Keep adding to final report draft.
* Fine-tune poster presentation.
* Literature Review.
