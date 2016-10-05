# Unix Utilities

_More powerful than the spiky blue shell_

## Challenges

Challenges within each section are meant to be solved in order.

### Navigation

1.  `pwd`
1.  `ls`
1.  `ls *.txt`
1.  `ls project`
1.  `cd project`
1.  `cd ..`
1.  `cd path/to/project`
1.  `cd ~` (or `cd`)
1.  `cd -`

### Variables

1.  `echo "Hello world"`
1.  `echo $USER` or `echo $PATH`
1.  `NAME=Firstname`, then `echo $NAME`
1.  `FULLNAME="Firstname Lastname"`, then `echo $FULLNAME`
1.  `env`
1.  `alias hello='echo "Hello world"'`
1.  `alias`
1.  `bash --help`
1.  `man echo` or `man ls`

### Files

1.  `cd animals`
1.  `cat cats.txt`
1.  `cat cats.txt dogs.txt`
1.  `wc cats.txt`
1.  `wc *.txt`
1.  `cp dogs.txt baby_dogs.txt`
1.  `mv baby_dogs.txt puppies.txt`
1.  `mkdir shelter`
1.  `mv puppies.txt shelter`
1.  `cp cats.txt shelter/kittens.txt`
1.  `rmdir shelter`
1.  `ls shelter`
1.  `wc shelter/*.txt`
1.  `rm -i shelter/*.txt`
1.  `rmdir shelter`

### Permissions

1.  `whoami` (or `echo $USER`)
1.  `ls -l *.txt`
1.  `chmod a+w cats.txt`
1.  `ls -l cats.txt`
1.  `chown otheruser cats.txt`
1.  `ls -l cats.txt`
1.  `chown $USER cats.txt` or `chown $(whoami) cats.txt`
1.  `sudo chown $USER cats.txt` (or `sudo !!` but be careful)
1.  `ls -l cats.txt`

### Streams

1.  `echo "Hello world" > test.txt`
1.  `echo "Hola Mundo" >> test.txt`
1.  `cat test.txt`
1.  `cat numbers.txt`
1.  `head numbers.txt`
1.  `head -n 5 numbers.txt`
1.  `tail numbers.txt`
1.  `tail -n 5 numbers.txt`
1.  `head -n 10 numbers.txt | tail -n 5`
1.  `sort numbers.txt`
1.  `cut -c 1-2 numbers.txt`
1.  `cut -c 1-2 numbers.txt | sort`
1.  `cut -c 1-2 numbers.txt | sort | uniq`
1.  `tr o 0 test.txt` (or `sed -e 's/o/0/' test.txt`)
1.  `tr a-z A-Z test.txt`
1.  `echo "Hello world" | tr a-z A-Z`

### Search

1.  `find animals -name cats.txt`
1.  `find ~/code -name '*.py'`
1.  `find ~/movies -size 100M`
1.  `grep 'one' numbers.txt`
1.  `grep 'def search' ~/code/search.py`
1.  `find ~/code -name '*.py' | grep 'def search'`
1.  `find ~/code -name '*.py' | xargs | wc`
1.  `grep '[0-9]{5}' ~/addresses.txt`
