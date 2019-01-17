namenode重新初始化后或IP改变了，datanode 无法重启，检查 `/hadoop/hdfs/data/current` 下的 VERSION 和 namenode `/hadoop/hdfs/namenode/current/VERSION` 是否一致，不一致，删除 datanode 的文件

```
# cd /hadoop/hdfs/data/current
# rm -rf *
```
