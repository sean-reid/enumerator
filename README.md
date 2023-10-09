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

## setup
the prerequisites of running `enumerator` are:
* git
* python3.8 or higher
* this repository

to install git and python3.8 (MacOS), use [Homebrew](https://brew.sh):
```
brew install git python3.8
```

to install git and python3.8 (Ubuntu), use `apt-get`:
```
sudo apt-get update
sudo apt-get install git python3.8
```

to install git and python3.8 (Windows), use [Chocolatey](https://chocolatey.org/install):
```
choco install git.install python --version=3.8.0
```

to clone the repo:
```
git clone https://github.com/sean-reid/enumerator.git
```

before running the script, change into the repo directory:
```
cd enumerator
```

you can also make a virtual environment if you'd like:
```
python3.8 -m venv .venv
source .venv/bin/activate
```

## usage
call enumerator with something like the following:

```
./enumerator --size 4 --ones 3 -v
```

this will count all 4x4 matrices with 3 ones in every row and column.

the -v flag will save all valid matrices to a timestamped log file, named `<timestamp>-enumerator.log`.

## author
* [sean reid](sean-reid.github.io)
