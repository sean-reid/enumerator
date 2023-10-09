# enumerator
counts the number of binary NxN matrices which have exactly M ones in every row and every column with a brute force approach

## example
if N = 4 and M = 3, then a valid matrix could be:

```
0 1 1 1
1 1 1 0
1 0 1 1
1 1 0 1
```

for N = 4 and M = 3, the following matrix would be invalid:

```
0 1 1 0
0 1 1 1
1 1 1 1
1 1 0 1
```

the above is invalid because the first row and the first column have only 2 ones, and the second column and third row have 4 ones.

# usage
call enumerator with something like the following:

```
./enumerator --size 4 --ones 3 -v
```

the -v flag will save all valid matrices to a timestamped log file, named `<timestamp>-enumerator.log`.

## author
* [sean reid](sean-reid.github.io)
