# check if a datastructure or method is there in Python to do the task effectively.
# First google the task you want to do in numpy or pandas and check if it can be done in a single method.
# Know your datastructures. Check which data structure can do faster processing.
# Explore the various methods thata re available to do your computation.
# compare with the execution time needed for that operation against that method.





# Find common elements between 2 arrays or lists

## Sets : Sets - store unique values
list(set(list1) & set(list2))
    OR
set(list1).intersection(set(list2))
### convert lists to sets 
        list: Imagine you are looking for your socks in your closet, but you don't know in which drawer your socks are, so you have to search drawer by drawer until you find them (or maybe you never do). That's what we call O(n), because in the worst scenario, you will look in all your drawers (where n is the number of drawers).

        set: Now, imagine you're still looking for your socks in your closet, but now you know in which drawer your socks are, say in the 3rd drawer. So, you will just search in the 3rd drawer, instead of searching in all drawers. That's what we call O(1), because in the worst scenario you will look in just one drawer.

## numpy.intersectid method
numpy.intersect1d(array1,array2)

## Convert the datastructure to numpy array
    numericlist = numpy.array(stringlist).astype(int)
    ## apply conditions
    numericlist[numericlist <conditional operator> value].method()
      e.g: numericlist[numericlist < 25].sum()