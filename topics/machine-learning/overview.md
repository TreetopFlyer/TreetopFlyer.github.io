- Learning as Approximation
http://stat.smmu.edu.cn/history/pearson1901.pdf
Machine learning is a set of tools for examining point clouds to determine their overall shape, making it similar to linear regression and curve-fitting.
If you have heard about artificial intelligence/machine learning in passing, this may come as a surprise, and probably a disappointment. It's a worthwile topic to look into, it's just not what people make it out to be.

Given a table of observational data, if we take each column in a row to be the coordinates of some point, we attempt to classify this data point simply by looking at the region of space that the point occupies. The idea being that data points of similar real-world observations will "live" in similar regions of space.

A good example might be with something like weather data. If we make daily observations of 5 variables (wind speed, temperature, humidity, visibility, and pollen) for a year at a location. We then take only the Winter data and figure out the region (in 5 dimensional space) that those points live in --and we do this for each of the four seasons.
Then, given a new 5 dimensional weather observation, without being told the time of year, we can infer when it happened by checking which of the four regions it is in. There may be some overlap in the regions, so we can just return a value for how far the point is in each region, so an observation in late spring might return: [winter:0.01, spring:0.7, summer:0.6, fall:0.02]

So we need a way to mathematically define these regions. The region has to, if need be, take on a shape that is more complex that a square, circle, or dividing line. It also has to be able to do this in N-dimensional space. It turns out that matricies, or a series of matricies, can do this pretty well.


- Machine learning as a series of tests
A matrix subjects a set of points to an "affine transformation." This is a basic change in the shape of the 


- The biological plausibility of machine learning methods

Frank Rosenblatt's contribution to machine learning was approximating the behavior of a biological neuron as the dot product ran through a limiting function. He put too much faith in our ability to model real brains and we can debate his ideas all day by casting doubt in examining the *highly* nuanced behavior of real biological neurons, but he is the one that started all this and his model is as simple is it is useful, that much is not up for debate.

Teuvo Kohonen's contribution was noting that neurons live in layers and the layers and the layers have neighborhoods of cells that have similar weights. We can pan his observations noting that they rely on distance calculations

- The conciousness problem
the output of a machine is the test results. there is no mechanism that gives rise to conciousness. this is bad because the one thing i know in life for sure is that i am concious