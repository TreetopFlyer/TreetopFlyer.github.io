
- ML was for me, too hard to research. I want to make it as easy as possible for others like me to understand.
After researching and building various artificial networks as a layperson, a dunce even, I feel compelled to just talk about machine learning in the simplest, non-mathematical terms possible.
The overly abundant, overly technical ramblings on the subject that circulate the internet do little to help regular people with their curiosity.
It is a great irony that machine learning's champions are apprently such enemies of human learning, something they were trying to re-create in the first place!

- In the real world ML is about modeling probabilities and not building a software version of the brain.
For the record, the majority of machine learning applications end up being statistcs tools.
Still on the record, the authors of these tools did *not* observe the brain at the neurological level, learn exactly what it was doing in it's entirety,
then re-create what they saw in software form, and now we have computers that can replace people.
No one knows what the whole brain is really doing, and at this rate, we will probably never know what kind of machine gives rise to conciousness.

- Usually ML applications are just clever uses of matricies.
We will consider different artificial networks to simply be a variety of software that similarly perform a series of "stencil checks" on an input to determine it's nature.
I use the term "stencil check" and will continue to elaborate on this, but an even more familiar way of thinking about this would be a typical TV talent show.
A performer acts in front of a panel of experienced judges, and each gives their own grade of the performance. This collection of which judge said what tells us a lot about what is going on.
This is the most non-mathematical way I can think of to describe what a matrix is and does. If a person is like a vector, then a matrix is like a commitee of people.
When presented with a vector, the matrix returns a list of grades indicating how similar the observed vector is to each vector within the matrix, effectively "classifying" it.
The way we go about doing ML on a computer is we take vectors and run them through matricies to see what was output.

If you are already familiar with matricies, you are probably pretty indignat right now and want to know what the difference between machine learning and a plain-old matrix transformation is.
The answer is not much. There are definately some bells and whistles added, but a lot of ML boils down to figuring out what vectors should be in the matrix.

- Matricies are, in part, biologically plausible.
A big question is, is this not biologically correct?
We *can* argue that groups of biological neurons are indeed performing "stencil checks" through their receptive fields and that these neurons can adjust their stencils to be more like something they encounter often.
It is also more-or-less known that the way we regonize things has to do with the output of several layers of neuron groups in series.
But it is at this point that ML diverges from the biological and is not concerned with creating an accurate brain simulation, but instead seeks useful ways of classifying real data.



- Self Organizing Maps
We begin with Self Organizing Maps, as they
mimic some great biological behaviors (so-called "competative learning"),
are very easy to understand,
do not required "labeled" data,
can help tremendously with visualizing very high dimensional data by arranging it on a 2d surface,
and they can easily be stacked into layers to produce more high-level interpretations of data.
Other than relying too much on distance calculations, there's a lot to like here, and they should be useful to just about anybody.
A similar and more popular algorithm known as k-means exists, but k-means does not produce as elegant of an output and is a little more "crude" all-around.