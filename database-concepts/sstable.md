A storage format that is used when saving data to disk that first appeared in Google's Bigtable Paper. It is a sequence of key-value pairs sorted by key.

From BigTable's paper:

> Internally, each SSTable contains a sequence
of blocks (typically each block is 64KB in size, but this
is configurable). A block index (stored at the end of the
SSTable) is used to locate blocks; the index is loaded
into memory when the SSTable is opened. A lookup
can be performed with a single disk seek: we first find
the appropriate block by performing a binary search in
the in-memory index, and then reading the appropriate
block from disk

Technologies:

- BigTable
- HBase
- Cassandra
- LevelDB
- RocksDB
