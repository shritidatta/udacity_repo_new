# Renaming columns
## method 1
new_df = old_df.rename(columns ={'old colname1': 'new colname1', 'old colname2': 'new colname2', 'old colname3': 'new colname3'})

## method 2 --- if just a space ' ' to be replaced with '_'
labels = list(old_df.columns)
labels[0] = labels[0].replace(' ', '_')
labels[1] = labels[1].replace(' ', '_')
labels[2] = labels[2].replace(' ', '_')
old_df.columns = labels

## OR

df.columns = [col.replace('', '_') for col in df.columns]       

# Feature Analysis
## Median value for a feature and setting a threshold 
### value >= median = 'high'  ,  value < median = 'low'
## observing the mean quality rating for the top and bottom half of each feature
median_value = df.'columnname1'.median()

for i, 'columnname1' in enumerate(df.columnname1):
    if columnname1 >= median_value:
        df.loc[i, 'columname1'] = 'high'
    else:
        df.loc[i, 'columnname1'] = 'low'

df.groupby('columnname1').columnname2.mean()    

df.groupby(['columname1','columname2']).mean()

### OR --- generalize it

def numeric_to_buckets(df, columnname):
    median = df.columnname.median()
    for i, val in enumerate(df[columname]):
        if val >= median:
            df.loc[i, columname] = 'high'
        else:
            df.loc[i, columname] = 'low'   

### calling the function - setting a range
for col in df.columns[:-1]:
    numeric_to_buckets(df,col)
    print(df.groupby([col]).quality.mean())

# Read files
with open('<filename>') as file:
    recent_data = file.read().split('\n')

# System time
starttime = time.time()    
executiontime = time.time() - starttime

# Intersections between 2 lists (arrays)
    # numpy - intersect1d() method
        numpy.intersect1d(list1, list2)

    # Set
        list(set(list1) & set(list2))
            OR
        set(list1).intersection(set(list2))    

# Strings to integers - conversion
numpy.array('string').astype(int)

# Numpy index - seperation  with condition
intarray[intarray <conditionaloperator> value].<operation>
    eg: intlist1[intlist1 < 25].sum() * 1.08

# main
if __name__ = "__main__"
    A main bloc is run when a code file is directly run. It will not help to import the functions that are in this file.



