# Notes on the Midterm

* _Correctness    (out of 40):_ 40
* _Good Practices (out of 10):_ 9
* _Docs / Testing (out of 10):_ 10

_Details on the grading criteria for the midterm can be found on [Canvas](https://canvas.slu.edu/courses/28045/rubrics/23671)._

Overall, nice work on using comments and tests in your docstrings!

I instructed the midterm to be put in a folder on github.com, but you left yours at the root of your project. No points off for that since it was obvious where it was.


## Step 1
* Nice work.  Note that when you've called json.load(), it's done reading the file. You can unindent your code below that line because it doesn't need to be in the `with` block.
* You are computing the `sum_rates` and `avg_rates` during every iteration of the loop, but could have saved that until the last step right before returning the average. I've subtracted 1 point from _Good Practices_ for this.

## Step 2
* Your code here isn't going to exactly what you think it is because your `else:` statement is unindented from the `if` statement.  I'm surprised it even runs that way! I guess that Python just never gets to the `else` statement based on how you've written it.
* Take care that you want to return None at the very end of looping through everything. Only at the very end will you know that what you're looking for is not there.

## Step 3
* No additional comments.

## Step 4
* You could have cleaned up the code a little bit by putting `if rate is not None: rate = 0` right after you get the adjusted rate.  Then you wouldn't have to repeat that code four times in your lower section. I've deducted 1 point from _Good Practices_ for this.
* Another style note, that variables with names that start with `_` are usually reserved for internal variables within a class; not generally used inside functions like this.