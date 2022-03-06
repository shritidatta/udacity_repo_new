# Writing Clean code:

## Meaningful names:
    # Be descriptive e.g: age_list
    # Impy type e.g: age_list
    # For boolean prefix with is_ or has_  e.g.: is_label
    # Use parts of speech - verbs for functions and nouns for variables e.g:
    # avoid useage of abbreviation 
    # avoid being verbose... long names != descriptive names
    # in functions - replace input arrayname with *arr*(arbitary array)
    e.g: def count_unique_values(name_list):   instead
        def count_unique_values(arr):

## Whitespaces and indentation:        
        *** PEP 8 style
    # Indentation - 4 spaces
    # seperate sections with blank lines
    # limit lines to 79 characters   

## Modular code:
    # use numpy function
    # use less code (dont repeat yourself)
    # abstract out logic to improve readibility
    # minimize the number of entities (functions, classes, modules, etc.)
    # arbitary variables vi'z descriptive variable names
    # no more than 3 arguments per function


## Refactoring:

Refactoring: Restructuring your code to improve its internal structure without changing its external functionality.