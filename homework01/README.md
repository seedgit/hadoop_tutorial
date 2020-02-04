# Homework 01

Download Hadoop Single Node image (VMware or VirtualBox) to your machine ( : https://www.cloudera.com/downloads/quickstart_vms/5-13.html) 

Start virtual machine 

In your virtual machine. Download input file according to your student id from google drive lab01 folder (https://drive.google.com/open?id=1bPwLwW_3SgiEmEzECCEsH7Mt_fL9hzri) 

Make folder “/user/cloudera/lab01/input” in your HDFS 

Put your input file into 4) by using ```“hadoop fs –put localPath destPath”``` or ```“hadoop fs –copyFromLocal  localPath destPath"``` 

Write WordCount program to count word of your input file 

Download your output result using ```“hadoop fs –get hdfsPath localPath"``` or ```“hadoop fs –copyToLocal hdfsPath localPath"``` 

Change your output filename into format of your student id and type is “.out.txt” 

Submit your output file back to google classroom Hadoop Lab01  

## Hadoop Tip! 

You can use common Linux command (e.g, ls cat mkdir) by place it after “hadoop fs”  
E.g., hadoop fs –mkdir /user/cloudera/lab01 
