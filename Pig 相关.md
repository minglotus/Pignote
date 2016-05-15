#Pig 相关

* Pig出错时的log默认写入当前的工作目录
  so question comes: how to store pig log files into a separate directory?
  
  modification command:
  - in mapreduce mode
	```
      pig -l /log/path
     ``` 
  - in local mode
     ```
      pig -x local -l /log/path
      ```

* Pig 既可以操作HDFS上的数据，也可以操作本地数据
  load数据的命令
  ```
  load 'file-path' as table-name (column-name1: attribute1, ..., column-name n : attribute n)
  ```
