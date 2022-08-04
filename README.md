# bigdata-final

Catalyst Optimizer:

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
 


