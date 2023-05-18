# Geophysical-Tool-Response-Project
Geophysical Tool Response Project

## Initial idea

Given a field where you have data that has already been validated by an expert, gather a database to determine information clusters for expected values (for example Magsus, density, bmr, or any other tool response).


Train an algorithm to check new data that comes in and lets you know if the data you are gathering matches the same trends and let the user know whether he should get an additional opinion prior to departing from the hole that person is logging.

## Subsequent Expert Feedback

•	Curation of log data in a database
•	Calibration tracking with post-processing capabilities (knowing the all the algorithms)
•	Setting gates on channels based on tool specifications and, if we have a better understanding of holes logged geographically, gates set based on the distribution of expected values within a site
o	We have come across this before we could not be sure if low mag sus response was due to the tool or geology
 
Cluster analysis would be interesting by taking in all logging parameters as it may highlight domains based on specific tools or trucks or operators. This would definitely present, “warts and all”, the consistency of the data we are acquiring and delivering.
o	Again, a recent example is an operator noticing variation in mag sus baseline response depending on tool temperature through the day
 
So even taking a step back from “data that has already been validated by an expert”, pulling in all our production field data and performing some exploratory analysis along these lines would have value for us in my opinion.


## Additional Ideas

we could start by plotting in a 2D plot Magsus vs Density or any other interesting curve. I suggest we try to see if we get something like the below:  that would give a very well-defined cluster of responses (that could be tied to some lithological property). We could then run a Kmeans or some other type of clustering algorithm to see if there are groups.

 
We could then add features like the temperature as a third dimension or fourth if we want to add more variables to see if the temperature moves the clusters in a particular direction. Maybe we can see clusters of sub-normal data for tools on their way out.

With the coordinate information we have available, we could potentially try and plot the same type of diagrams in different regions and generate a type of interactive report that provides info by location  

 
Each point could provide cluster information when clicked and could give an idea of the expected value per region

## More Feedback


I think the main challenge is determining whether any clusters are specific to the area logged vs. tool specific.

And then the question is: what do we want / can we predict?

The basic things I want to be able to do are:
-	Have a basic understanding of expected tool responses
o	This, of course, will be driven by geological domain, but let’s first see how consistent the data available is
-	How do tool calibrations track over time?
o	Focus on density and mag sus
-	Can a “baseline” tool response be defined across the entire dataset?
o	Are there fluctuations through each day / over time?
o	Are some tools noisier than others?
-	Can we look at active tool times and determine which tools are more “reliable”? Is “reliability” related to operator / truck?

 

