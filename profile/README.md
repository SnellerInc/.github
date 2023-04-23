Sneller is a high-performance SQL engine built to analyze
petabyte-scale un-structured logs and other event data.

Here are a couple major differentiators between Sneller and other SQL solutions:

 - Sneller is designed to use cloud object storage as its **only** backing store.
 - Sneller's SQL VM is [implemented in AVX-512 assembly](https://sneller.io/blog/2023/03/22/sql-vm-in-avx-512/).
   Medium-sized compute clusters can provide throughput in excess of **terabytes per second**.
 - Sneller is [completely schemaless](https://sneller.io/blog/2023/03/21/why-schemaless/).
   No more ETL-ing your data! Heterogeneous JSON data can be ingested directly.
 - Sneller uses a [hybrid approach between columnar and row-oriented data layouts](https://sneller-dev.io/blog/2023/03/27/zion-format/)
   to provide lightweight ingest, low storage footprint, and super fast scanning speeds.

[Sneller Cloud](https://console.sneller.io/register) gives you access to a hosted version of the Sneller SQL engine
that runs directly on data stored entirely in **your S3 buckets**.
Our cloud platform offers excellent performance and is priced at an extremely competitive \$150 **per petabyte** of data scanned.
