# Hapax-Legomena
A program that lists the hapax legomena from a given data file
Our tool will tally how many occurrences of each word there are in each data file presented on the command line, but our
underlying objective is to list the hapax legomena. Each hapax legomenon (the singular form of this term) is a word that
occurs only once in an entire document
# Intended Program Function
Our program will take information from the command line in order to determine how it operates. The usage key for our
program is this:
```
Usage:
  hapax [<options>] <datafile> [ <datafile> ...]
Options:
-d     : print out all data loaded before printing hapax legomena.
-h     : this help. You are looking at it.
-l <N> : only print hapax legomena of length <N>.
       : If no -l option is given, all hapax legomena are printed.
```

Running the program will print out the hapax legomenon from one or more data files (of only the desired length if
indicated).

# Running The Program
After cloning the repository run the comman ```make``` followed by

```./bin/hapax [<options>] /src/data<datafile> [<datafile> ...]```
The use of [ ] brackets indicates an optional item, and items in < > brackets
indicate a value. This means that the above is saying that all of the options are, well, optional; the “<datafile>” arguments
can optionally be in a list with many filenames; and the “-l” argument takes a number following the argument as a value
indicating the length.