## 

1. Create flume configuration file
2. Apply your twitter key
3. Run flume to get data from twitter 

```flume-ng agent --conf ./conf/ -f conf/twitter.conf Dflume.root.logger=DEBUG,console -n TwitterAgent```
4. Write MapReduce program to analyze that data

