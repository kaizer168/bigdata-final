# bigdata-final

Catalyst Optimizer:

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#37L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#150L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#227L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#284L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#325L] 
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#442L]      
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#467L]      
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#488L] 
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#581L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#662L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#783L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#868L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1009L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1150L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1247L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1348L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1457L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1474L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1603L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1664L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1693L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1710L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1755L]
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 Aggregate [count(1) AS count#1816L]

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1828L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true

=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1844L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1860L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, trueOverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true 
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1876L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true 
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1892L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1908L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, trueOverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1924L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ReorderJoin ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ColumnPruning ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.NullPropagation ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.ConstantFolding ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.InferFiltersFromConstraints ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.PushDownPredicates ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true
 
=== Applying Rule org.apache.spark.sql.catalyst.optimizer.RewritePredicateSubquery ===
 OverwriteByExpression RelationV2[] noop-table, true, true
 OverwriteByExpression RelationV2[] noop-table, true, true
 +- Sort [cnt#1940L DESC NULLS LAST], true

