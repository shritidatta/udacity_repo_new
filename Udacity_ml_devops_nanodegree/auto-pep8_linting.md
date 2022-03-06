# Key Points
Once you have a working solution in a notebook, it is useful to make your code reusable by creating a function.
You can then add a if __name__ == "__main__" block to your script to be run for testing or showing how the functions in your script work.
Running your script from the terminal can be done with ipython script_name.py or python script_name.py

    def all fiunctions defined above:
        return values
    if __name__ == "__main__"
        call function
        print result

# Two ways to automate clean code are with
    pylint
    autopep8
        pylint script_name.py will provide feedback on updates to make to your code, as well as a score out of 10 that can help you understand which improvements are most important.
        autopep8 --in-place --aggressive --aggressive script_name.py will attempt to automatically clean up your code.        