## 查询集群

### 负责

1. 接受用户查询；

2. 维护查询信息；
   
   1. 查询内容；

   2. 查询涉及到的索引节点；
   
   3. 查询涉及到的聚集节点；

3. 聚集最终结果；
   
   1. 维护一个容量为k的堆；

## 索引集群

### 负责

1. 保存索引；

2. 内节点负责根据查询返回相关的子节点；

3. 叶节点负责根据查询返回相关的聚集节点；

4. 叶节点负责向聚集节点发送本节点中的关键字频率信息；

## 聚集集群

### 负责

聚集关键字并向查询集群发送局部聚集结果；

## 优化

1. 空间划分
