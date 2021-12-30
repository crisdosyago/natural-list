# natural-list

A self-organizing list that naturally obtains an optimal length

# Inspiration, Motivation and Idea

Actually that should probably be motivation, inspiration and idea.

Motivation:

![idea](https://user-images.githubusercontent.com/22254235/147742669-8946ecb2-9ad8-4ac6-8698-a968471d6bc8.PNG)

The Google Chrome "add bookmark" UI, select folder option, brings up a dropdown (or brings down a dropdown?, or drops a dropdown?...) that is always ended with 3 staples (Bar, Mobile and Other -- the three "roots"), and then has 4 or 5 places on top of that for the most commonly (or most recently) used items. So it's like the head of a least recently used cache. 

But here's the problem, which is the motivation for this library...I never feel it keeps "enough". 4 or 5 is simply not enough for me if I'm commonly operating under 8 - 10 categories, four or five free spots will mean that other equally recently or commonly used categories will keep being pushed out and then necessitate a click-expensive hunt behaviour, where I need to do a few more clicks and perform some elaborate search and discovery folder opening and closing, scrolling or searching across the "Bookmark Tree" (rather, that should be "Bookmark Forest" not because it's a mathematical forest with many separated trees...but simply because it's as hard to find something in a large collection of bookmarks as trying to find something in a forest.)

So I realized this would be better if the list expanded and shrank to encompass (not all) but "most" of the categories I am recently using. Why should it be a fixed number of slots? Everyone has different organizing habits, and certainly even changes their organizing habits at different times. So a real natural list, should be able to adapt to that.

Inspiration:

This part is fairly vague right now but I just had a flash of insight, a sense that this could be somehow done mathematically. That there should both be a natural way to decide a "time window" on which to assess the range of categories used (and in which to try to represent the most common categories), and also to, for such a time window, decide the number (and the instances) of the categories "common" in that window. These values, timeWindow, commonCategoryCount, and commonCategoryNames, should be all calculable from the human's behavior somehow, in a way that can achieve some optimal property relevant to usability, and particularly the case I describe above. 

Idea:

Not sure yet on specifics, but could it have something to do with using probability distributions? Perhaps probability distributions relevant to nested categories arranged as trees?
