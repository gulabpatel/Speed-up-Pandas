Pandas cannot handle more than a few GB of data.

I am not the only one, even the creator Wes McKinney thinks so.

In his talk "10 things I hate about Pandas," he describes 11 reasons he does not like about Pandas:

1. Internals too far from "the metal"
2. No support for memory-mapped datasets
3. Poor performance in database and file ingest / export
4. Warty missing data support
5. Lack of transparency into memory use, RAM management
6. Weak support for categorical data
7. Complex groupby operations awkward and slow
8. Appending data to a DataFrame tedious and very costly
9. Limited, non-extensible type metadata
10. Eager evaluation model, no query planning
11. "Slow", limited multicore algorithms for large datasets

Instead of using Pandas, use these suggested packages.

👉Dask: a low-level scheduler and a high-level partial Pandas replacement, geared toward running code on compute clusters.

👉Ray: a low-level framework for parallelizing Python code across processors or clusters.

👉Modin: a drop-in replacement for Pandas, powered by either Dask or Ray.

👉Vaex: a partial Pandas replacement that uses lazy evaluation and memory mapping to allow developers to work with large datasets on standard machines.

👉RAPIDS: a collection of data-science libraries that run on GPUs and include cuDF, a partial replacement for Pandas.

If those do not work, try #spark.
