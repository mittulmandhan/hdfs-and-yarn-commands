# HDFS And YARN Commands
## HDFS Commands
* hdfs -help
* hdfs namenode -format
* start-all.sh 
	(depricated)
* start-dfs.sh
* start-yarn.sh
* jps
* hdfs dfs -ls /
* hdfs dfs -help
* hdfs dfs -put <local-file-location> <hdfs-paste-location>
* hdfs dfs -copyFromLocal <local-file-location> <hdfs-paste-location>
* hdfs dfs -put <local-file-location> <hdfs-cluster-url>
* hdfs dfs -get <hdfs-file-location> .<local-paste-location>
* hdfs dfs -copyToLocal <hdfs-file-location> .<local-paste-location>
* hdfs dfs -mkdir /<directory-name>
* hdfs dfs -mv <file> <move-location>
* hdfs dfs -setrep <replication-factor> <dir-location/file-location>
* hdfs dfs -touchz <file-name-with-location>
* hdfs dfs -cat <file-name-with-location>
* hdfs dfs -stat "<attributes>" <file-name-with-location>
* hdfs dfs -appendToFile <localsrc> ... <dst>
* hdfs dfs -getmerge <hdfssrc> ... <localdst>
* hdfs dfs -test -[edsz] 

## HDFS Admin Commands
* hdfs dfsadmin -safemode <enter | leave | get | wait>
* hdfs dfsadmin -report [-live] [-dead] [-decommissioning]
* hdfs dfsadmin -printTopology
* hdfs dfsadmin -<setQuota | clrQuota> /mydir
* hdfs dfsadmin -<setSpaceQuota | clrSpaceQuota> /mydir <size-in mb>
* hdfs dfsadmin -getDatanodeInfo 127.0.0.1:50020

## YARN Commands
* yarn jar <your-jar-file> <CLAUSE>
* yarn application -list -appStates <appStates-parameters> -appTypes <appTypes-parameters>
* yarn application kill <application-ID>

Note: All the commands are case sensitive.
