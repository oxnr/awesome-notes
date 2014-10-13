1. Distributed File Systems

1.1 Problems
Persistant availability if nodes fail
Network bottlenecks
Distributed programming is complex

1.2 Examples
Google GFS, Hadoop HDFS

1.3 Functionality
Data kept in spread "chunks" and replicated through multiple machines
Chunk servers also act as compute servers (avoid data movement)
File is split into contiguous chunk (16-64mb) and is replicated 2-3x
Master node stores metadata about where the files are stored
Client talks to master to find chunks and then directly talks to chunk servers

2. Map-Reduce Computational Model

Map and Reduce tasks can be specified by the developer

2.1 Map
Scan input file record-at-a-time
Extract something your care about from each record (key)

2.2 Group by key
Sort and shuffle

2.3 Reduce
Apply a reduce step (Aggregate, summarises, filter or transform) and write results

The reads are sequential reads (not random access) why it's very efficient

3. Scheduling and Data Flow

3.1 Scheduling
All phases are distributes with many tasks doing the work in parallel
M.R. takes care of partitioning, scheduling, group by key, failures and whole communication

3.2 Data Flow
Input and final output are stores on the distributed file system
Scheduler tries to schedule map tasks close to physical storage of input
Intermediate results are stored on local FS of Map and Reduce workers
Output is often input to another tasks

Master node takes care of coordination such as task status and idle tasks

If a map-worker fails the worker is reset to idle and the tasks eventually needs to be reschedules on other workers

Rules of thumb
A. Make m much larger than number of nodes
B. One DFS chunk per map is common
C. Improve dynamic load balancing and speed up recovery from worker failures

4. Combiners and Partition Functions

4.1 Combiners

4.2 Partition Functions

5.  Link analysis & Page rank

Graph data
