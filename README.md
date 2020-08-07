# challenge-ruby
#
# Refactoring Challenge

During support we sometimes write some quickfix solutions, which we think will
not be needed apart from that one time task. Thus the code usually has no
tests, is not documented and just everything in one large file. Attached you
find an example for such an assumed one time task - modifier.rb.

Please do the following:

- give a short explanation of what the code actually does.
- refactor the code and ensure that the refactored code does the same
  as before.
- create a git repository containing the initial files and do regular
  and small commits to log your process.
- send me your git bundle containing your changes.

# A summary of what I found out about this challenge.

-the latest method is called, which takes a string as an argument and finds each file in a special folder that has this title in its name and these files are based on the date in the name.
They are sorted and then returned. Last file date ...
The first step is to call the input sort method, in which the file is read as CSV and its contents and headings are separated.
Then in write method, all data and headers are added to the variable and sent to the sort method, which will also be the result of the sort method.
The result of the last steps is sent as an argument for lazy reading, where each line is read as CSV.
The data read for the Combiner class hybrid method would be an argument to use csv data in each cell, instead of using other data (-1, 0, 1) and sending an array. To modify the method, it is stored in a variable called combiner.
Each combiner element is process in a method called Combine_hashes, in which a hash is created  and  stored in a variable called Merge.
inally, the merged data is placed in a csv file with the same name as the input file, followed by a list starting from zero, and in each file there are up to 120,000 data lines, and if there is more information. You save it in another csv file in the same directory, only its index changes and increases by one index to make a difference between the files.