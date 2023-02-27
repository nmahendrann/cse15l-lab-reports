# Lab Report 3


## Grep commands

* One command is the -w, which returns only if the string is a word and not part of a word
```
$ grep -w 'success' *
HistoryEgypt.txt:        Limited success in 1973 restored some national pride when the Sinai was
HistoryHongKong.txt:        Japanese Christians. While Christianity was not a great success in
HistoryIbiza.txt:        ensured its continued success.
```
```
$ grep -w 'mistake' *
WhatToLasVegas.txt:        Make no mistake: the times may be changing, but without gambling, there
```
* This method returns the line and file only if the inputted string is a standalone word. This is useful when searching for certain tenses or searching for specific sections based on keywords.

* Another command is the -i, which isn't case sensitive for the inputted string
* These commands were done inside the berlitz one directory

```
$ grep -i 'ocho rios' *
HandRJamaica.txt:        Ocho Rios
HandRJamaica.txt:        views of the sea, located a short way out of the center of Ocho Rios.
HandRJamaica.txt:        Ocho Rios; Tel. 974-2201, 974-2219; fax 974-2289; e-mail
HandRJamaica.txt:        Ciboney Ocho Rios ❁❁❁❁❁ (AI) P.O. Box 728, Ocho Rios; Tel.
```

```
HistoryMalaysia.txt:        north coast of Borneo and the east coast of the peninsula, and
IntroMadeira.txt:        cooler north coast, you will see terraces of bananas and vines that
WhatToJamaica.txt:        Montego Bay, Ocho Rios, and the North Coast
```

* These are not the only files returned, but this command prints the line with the inputted string along with the file its in. It doesn't check for capitalization, which could be usefule when searching for passwords or something with random cases.


* Another command is -l, which shows the filenames of the files that matched
* These commands were done in the berlitz one directory

```
$ grep -l 'history' *
HistoryDublin.txt
HistoryEdinburgh.txt
HistoryEgypt.txt
HistoryFrance.txt
(more files were printed too)
```

```
$ grep -l 'death' *
HistoryDublin.txt
HistoryEgypt.txt
HistoryFrance.txt
HistoryGreek.txt
```
* This command prints the files in which the word is located. This is useful when searching for specific evidence. The word can be used to find the files with the most benefecial information.

* Another command is -o, which only prints the matching part of the line, not the whole line
* To use this, the directory was changed to berlitz one

``` 
$ grep -o 'the' IntroEgypt.txt 
[the] was printed 124 times
```
 

```
$ grep -o 'help' HistoryGreek.txt
help
```

* This command option prints the specific string in the input, and not the whole line. This is useful for counting the amount of times a word was used in order to have a variation in diction or check fro redundancy.



* The commands were found in [wizardzines](https://wizardzines.com/comics/grep/)
* The functions of the code were discovered through chatGPT, and then experimented with in VSCode
