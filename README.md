# word-count-mapreduce
Here Word Count using Hadoop MapReduce is implemented

### Steps for Execution ###

1. Start Hadoop System on your machine<br />
    *check if all the daemons have started using 'JPS' command*
2. Make Directory “WordCountProgram” in HDFS. Make a directory “Input” in “WordCountProgram”. Add “input.txt” File in the “Input” Directory that was created before.
3. Create a directory Word_Count_Classes for storing the class files of “WordCount.java”. Execute commands shown Below.
4. Create a Jar file using following commands:<br />
    *jar cvf WordCount.jar 'WordCount$IntSumReducer.class' 'WordCount$TokenizerMapper.class' 'WordCount.class'*
6. Now run the program using Hadoop<br />
    *hadoop jar 'your jar file path' WordCount /WordCountProgram/Input /WordCountProgram/Output*
7. Run cat command to view results stored in “/WordCountProgram/Output”<br />
    *hadoop dfs -cat /WordCountProgram/Output*

### Result ###
![Results](results.jpg)
