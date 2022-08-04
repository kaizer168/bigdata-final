# bigdata-final

毕业设计

题目一：分析一条TPCDS SQL

Q73 优化规则截图请看附件SQL-UI-1.png, SQL-UI-2.png, SQL-UI-3.png, SQL-UI-4.png, SQL-UI-5.png, SQL-UI-6.png, SQL-UI-7.png.

Q73 使用了优化规则 Catalyst Optimizer:

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
 
PushDownPredicates 谓词下推这条优化规则的思路是把Filter过滤条件尽可能往下推到靠近数据源的位置，这样可以先把数据量在查询开始后尽可能早的的开始缩减，直接跳过无关的数据，只读取需要的数据，再进行其他计算，从而减少了后续聚合时需要处理的数据量，有效减少数据加载的I/O操作，还有减少内存资源和计算资源的开销，並提高查询效率。谓词可以是一个表达式或者涵数，相对应SQL WHERE之中的表达式，可以是true或者false值，在优化过程中被判定是否通过谓词测试。若要遍历整个数据集，可能只用到其中一部份数据，如果没有谓词下推这条优化规则，会导致I/O和CPU的大量浪费。

ColumnPruning 列裁剪是指只读取需要的列，以此实现高效的列数据扫描并减少了I/O操作。关系型数据库一般是通过二维表的方式来关理数据的，每一行代表一笔相关联的记录，每一列代表不同的数据属性。在使用这些数据的场景中，往往不需要全量的数据属性，只需要用到其中一些列。通过对数据进行列裁剪，将没有用到的列排除，就可以提取需要用到的列，这就是列裁剪的优化规则。类似谓词下推的优化规则操作，把需要的列信息往靠近数据源的位置下推，尽可能在读取数据源时将不需要的列排除掉，以减少网络和读取数据的I/O开销，同时减少后续操作的内存空间。

