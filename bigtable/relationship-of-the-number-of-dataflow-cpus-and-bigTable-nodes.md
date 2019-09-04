According to [Scio docs](https://spotify.github.io/scio/io/Bigtable), the number of cpus at Dataflow should be at most 3 times the number of BigTable nodes:

```
As a general note when writing to Bigtable from Dataflow you should at most use the # of Bigtable nodes you have * 3 cpus. Otherwise Bigtable will be overwhelmed and throttle the writes (and the reads)
```