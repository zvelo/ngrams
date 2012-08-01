ngrams
======

This is a ngrams package in C++, which can be used for character or word ngram analysis. It uses Ternary Search Tree instead of hashing table for faster ngram frequency counting. Words are converted to unique IDs and encoded to more compact base 256 integers.

It is a simplified implementation of Dr. Vlado Keselj's Text-Ngrams 1.6, which is a very flexible Ngram package in perl. See more information at http://users.cs.dal.ca/~vlado/srcperl/Ngrams/Ngrams.html


How to use it
-------------

1. download and save the source code.
2. `$> make`
3. `$> ngrams --type=word --n=3 --in= sample.txt` or `$> ngrams --type=character -n=3 --in= sample.txt`

That's it. If you found any bug or have any suggestion, please kindly send me email jerryy@gmail.com. Thanks.

Zheyuan Yu. Feb 18,2006


Revisions
---------

* Mar 28, 2005. Zheyuan Yu Modify ternary search tree to improve performance, save pointer of TstItems into vector, instead of saving TstItems. It will save some time when vector grows.
* Feb 18, 2006. Zheyuan Yu Initial implemenation
