# StackOverflow-with-Scala-and-Spark
implement a distributed k-means algorithm which clusters posts on the popular question-answer platform StackOverflow according to their score. Moreover, this clustering should be executed in parallel for different programming languages, and the results should be compared.

dataset: http://alaska.epfl.ch/~dockermoocs/bigdata/stackoverflow.csv

The motivation is as follows: StackOverflow is an important source of documentation. However, different user-provided answers may have very different ratings (based on user votes) based on their perceived value. Therefore, we would like to look at the distribution of questions and their answers. For example, how many highly-rated answers do StackOverflow users post, and how high are their scores? Are there big differences between higher-rated answers and lower-rated ones?

Resulting clusters:
  Score |  Dominant language | (%percent)  |  Questions
------- |------------------- |------------ | ----------
      0 |  Groovy            | (100.0%)    |       1631
      0 |  MATLAB            | (100.0%)    |       3725
      1 |  C#                | (100.0%)    |     361835
      1 |  Ruby              | (100.0%)    |      54727
      1 |  CSS               | (100.0%)    |     113598
      1 |  PHP               | (100.0%)    |     315771
      1 |  Objective-C       | (100.0%)    |      94745
      1 |  JavaScript        | (100.0%)    |     365649
      1 |  Java              | (100.0%)    |     383473
      2 |  Perl              | (100.0%)    |      19229
      2 |  MATLAB            | (100.0%)    |       7989
      2 |  Clojure           | (100.0%)    |       3441
      2 |  Python            | (100.0%)    |     174586
      2 |  C++               | (100.0%)    |     181255
      2 |  Scala             | (100.0%)    |      12423
      3 |  Groovy            | (100.0%)    |       1390
      4 |  Haskell           | (100.0%)    |      10362
      5 |  MATLAB            | (100.0%)    |       2774
      9 |  Perl              | (100.0%)    |       4716
     14 |  Clojure           | (100.0%)    |        595
     25 |  Scala             | (100.0%)    |        728
     36 |  Groovy            | (100.0%)    |         32
     53 |  Haskell           | (100.0%)    |        202
     66 |  Clojure           | (100.0%)    |         57
     78 |  Perl              | (100.0%)    |         56
     79 |  C#                | (100.0%)    |       2585
     85 |  Ruby              | (100.0%)    |        648
     97 |  Objective-C       | (100.0%)    |        784
    130 |  Scala             | (100.0%)    |         47
    139 |  PHP               | (100.0%)    |        475
    172 |  CSS               | (100.0%)    |        358
    212 |  C++               | (100.0%)    |        264
    227 |  Python            | (100.0%)    |        400
    249 |  Java              | (100.0%)    |        483
    377 |  JavaScript        | (100.0%)    |        431
    443 |  C#                | (100.0%)    |        147
    503 |  Objective-C       | (100.0%)    |         73
    546 |  Ruby              | (100.0%)    |         34
    766 |  CSS               | (100.0%)    |         26
    887 |  PHP               | (100.0%)    |         13
   1130 |  Haskell           | (100.0%)    |          2
   1269 |  Python            | (100.0%)    |         19
   1290 |  C++               | (100.0%)    |          9
   1895 |  JavaScript        | (100.0%)    |         33
  10271 |  Java              | (100.0%)    |          2
