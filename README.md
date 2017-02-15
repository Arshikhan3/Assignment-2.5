# Assignment-2.5
 Explain what is a cluster and what is a hadoop cluster
2.What is meant by a Rack and explain the rack arrangement in a hadoop cluster

Ans - CLUSTER: In a computer system, a cluster is a group of servers and other resources that act like a single system and enable high availability and, in some cases, load balancing and parallel processing.
In personal computer storage technology, a cluster is the logical unit of file storage on a hard disk; it's managed by the computer's operating system. Any file stored on a hard disk takes up one or more clusters of storage. A file's clusters can be scattered among different locations on the hard disk. The clusters associated with a file are kept track of in the hard disk's file allocation table (FAT). When you read a file, the entire file is obtained for you and you aren't aware of the clusters it is stored in.
Since a cluster is a logical rather than a physical unit (it's not built into the hard disk itself), the size of a cluster can be varied. The maximum number of clusters on a hard disk depends on the size of a FAT table entry.

Hadoop CLUSTER: A Hadoop cluster is a special type of computational cluster designed specifically for storing and analyzing huge amounts of unstructured data in a distributed computing environment. Such clusters run Hadoop's open source distributed processing software on low-cost commodity computers.
Hadoop clusters are known for boosting the speed of data analysis applications. They also are highly scalable: If a cluster's processing power is overwhelmed by growing volumes of data, additional cluster nodes can be added to increase throughput. Hadoop clusters also are highly resistant to failure because each piece of data is copied onto other cluster nodes, which ensures that the data is not lost if one node fails.
As of early 2013, Facebook was recognized as having the largest Hadoop cluster in the world. Other prominent users include Google, Yahoo and IBM.

RACK: A Node is simply a computer. This is typically non-enterprise, commodity hardware for nodes that contain data. Storage of Nodes is called as rack. A rack is a collection of 30 or 40 nodes that are physically stored close together and are all connected to the same network switch. Network bandwidth between any two nodes in rack is greater than bandwidth between two nodes on different racks.A Hadoop Cluster is a collection of racks.
Hadoop components are rack-aware. For example, HDFS block placement will use rack awareness for fault tolerance by placing one block replica on a different rack. This provides data availability in the event of a network switch failure or partition within the cluster.
Rack awareness is having the knowledge of Cluster topology or more specifically how the different data nodes are distributed across the racks of a Hadoop cluster. The importance of this knowledge relies on this assumption that collocated data nodes inside a specific rack will have more bandwidth and less latency whereas two data nodes in separate racks will have comparatively less bandwidth and higher latency.

The main purpose of Rack awareness is:

Increasing the availability of data block
Better cluster performance
 In simple words rack awareness is the strategy namenode employs to choose the nearest datanode based on rack information. 
