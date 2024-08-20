# MongoDB-Database-in-Edge-Computing-A-Performance-Evaluation
  This project is about benchmarking MongoDB database in edge computing setup in single-node and nine-node cluster.

  The study selects the Raspberry Pi (RPi) as an edge node because it constitutes a solid edge test device. Further, the study chooses the YCSB as a framework to benchmark MongoDB. It is regarded as one of the best frameworks to benchmark cloud systems due to its open-source, flexible, and extensible workloads. In addition, it loads the database with synthetic data that helps the developers gain standard benchmarking results.

The study aims to evaluate the performance of MongoDB in two different deployment setups of centralized and distributed environments using YCSB. The results help the developers to have a deeper insight into how MongoDB behaves with different applications in edge computing setup.

The experiments were conducted on two test scenarios single node and docker swarm cluster of nine RPi. 

Single node: In this scenario, we configured a single RPi with the docker containers of MongoDB and Mongo Express instances to simplify the management and deployment. YCSB has been directly installed on the device out of the docker containers. Figure 5 shows our test scenario 1 setup. 
With this configuration design, we load data sizes of 60000, 70000, 80000, 90000, and 100000 to MongoDB with workloads A, B, C, D, E, and F. Some of the experiments have been repeated 5 times to ensure the validity of our results. Workload A been benchmarked in test scenario1 125 times. The same is true for workloads B, C, and D each one has been benchmarked 125 times. The MongoDB has been loaded with 60000 data sizes for 100 times in total. The same is true for 70000, 80000, 90000, and 100000 data sizes each one has loaded 100 times. Throughput and RunTime are the key performance indicators that we collected from the YCSB results. The number of times that the throughput has been collected from the YCSB results is 500 times in total and the same is true for the RunTime.

  The single node setup data can be accessed through this link: https://github.com/SaraDanaKablTalabani/master_thesis/tree/main/raw_data/project_1/mongodb/single_node

  The following figures show the single-node setup:

  ![7](https://github.com/user-attachments/assets/99b6b1de-b7fb-4c59-9c76-c1aa39acbb10)



Docker swarm of nine nodes:
In this scenario, we configured nine RPis with the docker swarm containers of MongoDB and Mongo Express instances to form a cluster. YCSB has been separately installed on the manager node out of the docker containers. Figure 6 shows a general view of the distributed architecture of our setup.

With this configuration design, we load data sizes of 60000, 70000, 80000, 90000, and 100000 to MongoDB with workloads A, B, C, D, E, and F. Workload A been benchmarked in the first test scenario 250 times. The same has been done for workloads B, C, D, E, and F each one has been benchmarked 250 times. The MongoDB has been loaded with 60000 data sizes for 200 times in total. The same is true for 70000, 80000, 90000, and 100000 data sizes each one has loaded 200 times.


The cluster setup can be accessed through this link: https://github.com/SaraDanaKablTalabani/Databases_benchmarking_with_sharding/tree/main
The following figures show the nine-node setup:
  
![2](https://github.com/user-attachments/assets/aded9ec9-43d3-4df0-bc1f-613a4ac6d921)
