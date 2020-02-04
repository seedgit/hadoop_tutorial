# Homework 01

1. Download Hadoop Single Node image (VMware or VirtualBox) to your machine ( : https://www.cloudera.com/downloads/quickstart_vms/5-13.html) 

2. Start virtual machine 

3. In your virtual machine. Download input file according to your student id from google drive lab01 folder (https://drive.google.com/open?id=1bPwLwW_3SgiEmEzECCEsH7Mt_fL9hzri) 

4. Make folder “/user/cloudera/lab01/input” in your HDFS 

5. Put your input file into 4) by using ```“hadoop fs –put localPath destPath”``` or ```“hadoop fs –copyFromLocal  localPath destPath"``` 

6. Write WordCount program to count word of your input file 

7. Download your output result using ```“hadoop fs –get hdfsPath localPath"``` or ```“hadoop fs –copyToLocal hdfsPath localPath"``` 

8. Change your output filename into format of your student id and type is “.out.txt” 

9. Submit your output file back to google classroom Hadoop Lab01  

## Hadoop Tip! 

* You can use common Linux command (e.g, ls cat mkdir) by place it after ```“hadoop fs”```  
E.g., ```hadoop fs –mkdir /user/cloudera/lab01``` 
* Because we use virtual machine image from cloudera, you must run ```export HADOOP_CLASSPATH=$JAVA_HOME/lib/tools.jar``` in terminal before compile your java program
* You can compile code using ```hadoop com.sun.tools.javac.Main WordCount.java``` but be careful(for none java experience). Your class name must be the same as your file name. (e.g., WordCount.java must contain class WordCount)
* use ```jar cf wc.jar WordCount*.class``` to combine your compiled class into sigle jar file
* You can run your mapReduce program by using command ```hadoop jar wc.jar WordCount /user/cloudera/lab01/input /user/cloudera/lab01/output```
* For more information please visit hadoop official website (https://hadoop.apache.org/docs/r2.6.5/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html)[https://hadoop.apache.org/docs/r2.6.5/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html]). And be careful, to write java program, compile and run might be different depened on Apache Hadoop Version
