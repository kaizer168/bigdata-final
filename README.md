# bigdata-final

毕业设计

题目一：分析一条TPCDS SQL

Q73 优化规则截图请看附件sql-ui-1.png, sql-ui-2.png, sql-ui-3.png, sql-ui-4.png, sql-ui-5.png, sql-ui-6.png.

Q73 使用了以下优化规则 Catalyst Optimizer:

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
PushDownPredicates 谓词下推这条优化规则的思路是把Filter过滤条件尽可能往下推到靠近数据源的位置，这样可以先把数据量在查询开始后尽可能早的开始缩减，直接跳过无关的数据，只读取需要的数据，再进行其他计算，从而减少了后续聚合时需要处理的数据量，有效减少数据加载的I/O操作，还有减少内存资源和计算资源的开销，並提高查询效率。谓词可以是一个表达式或者涵数，相对应SQL WHERE之中的表达式，可以是true或者false值，在优化过程中被判定是否通过谓词测试。若要遍历整个大的数据集，但是可能只用到其中一部份数据，如果没有谓词下推这条优化规则，会导致I/O和CPU的大量浪费。

ColumnPruning 列裁剪是指只读取需要的列，以此实现高效的列数据扫描并减少了I/O操作。关系型数据库一般是通过二维表的方式来管理数据的，每一行代表一笔相关联的记录，每一列代表不同的数据属性。在使用这些数据的场景中，往往不需要全量的数据属性，只需要用到其中一些列。通过对数据进行列裁剪，将没有用到的列排除，就可以提取需要用到的列，这就是列裁剪的优化规则。类似谓词下推的优化规则操作，把需要的列信息往靠近数据源的位置下推，尽可能在读取数据源时将不需要的列排除掉，以减少网络和读取数据的I/O开销，同时减少后续操作的内存空间。





题目二：Lambda 架构

Lambda 架构将数据处理分成分成两条通路,一条是基于批处理的预计算，使用不可变的离线数据用批处理技术产生一些表,另一条是基于流处理的增量计算,通过流数据实时增长的方式处理产生一些表,再结合两条通路成为计算结果以提供实时查询的服务,根据查询的特点用离线查询或实时查询来访问这两条通路。这两条通路用不同的代码和不同的数据实现。批处理用来做最终的计算，或者是对历史数据重新计算来保证数据不丢失。流处理用来计算实时应用场景的趋势，对准确性要求不高。可以用流处理来计算当天的数据，再用批处理重新补偿历史数据。批处理把数据存储成为主要数据集,对预定的查询进行预计算,並产生各种视图以供查询。批处理调度之间的空隙而来不及处理的增量数据可以由流处理来实时计算,一样可以产生各种视图以供查询。

请看附图Lambda-Architecture.png。批处理的存储方案可以是HDFS, S3。批处理的计算框架可以是MapReduce, Hive, Spark。批处理的计算结果可以存储在Hbase。流处理的计算框架可以是Flink, SparkStreaming, Storm。流处理的计算结果可以存储在高性能的内存数据库如Redis。

Lambda架构的优点是它提供了一种查询历史和实时大数据集合的可行模式。通过将数据处理分为批处理、流处理，即使在持续更新的大数据场景中，也能够获得包括历史和实时数据集合的查询结果。Lambda架构的缺点是对于同一个查询逻辑，需要为批处理和流处理开发不同的算法代码，测试和运维团队都要同时兼顾两套算法，因此出现了把批处理和流处理合并的Kappa架构。




毕业总结

大数据这门课学到了很多新的知识点。课程由浅入深，由最基础的Hadoop 到Hive，Spark，Flink，围绕着SQL on Hadoop 的主题，一层一层迭代, 覆盖了大数据知识体系的方方面面，探索了大数据的全貌。一些作业还是蛮有挑战性的，还好有助教的指点。Scala对我来说是新的编程语言，语法跟Java不尽相同，学了才能去看懂大数据项目原代码。现在学会了从GitHub下载开源代码，切换到特定分支，修改代码，编译跟测试，这些技巧肯定以后都会受用良多，学会了不吃亏。


