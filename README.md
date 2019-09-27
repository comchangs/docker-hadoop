# **hadoop**
___

### Description

This image runs the [*Cloudera CDH Hadoop*](https://www.cloudera.com/products/open-source/apache-hadoop/key-cdh-components.html) in a **pseudo-distributed** mode on a Centos 7 Linux distribution.

The *latest* tag of this image is build with the latest available release of CDH on Centos 7.

You can pull it with:

    docker pull comchangs/hadoop


You can also find other images based on different Apache Hadoop releases, using a different tag in the following form:

    docker pull comchangs/hadoop:[hadoop-release]-[cdh-release]


For example, if you want Apache Hadoop release 2.6.0 on CDH 5.11.1 you can pull the image with:

    docker pull comchangs/hadoop:2.6.0-cdh5.11.1

Run with Docker Compose:

    docker-compose -p parrot up


Once started you'll be able to read the list of all the Hadoop Web GUIs urls:

| **Hadoop Web UIs**        |**URL**                            |
|:--------------------------|:----------------------------------|
| *Hadoop Name Node*        | http://localhost:50070            |
| *Hadoop Data Node*        | http://localhost:50075            |
| *YARN Node Manager*       | http://localhost:8042             |
| *YARN Resource Manager*   | http://localhost:8088             |
| *YARN Timeline History*   | http://localhost:8188             |
| *MapReduce Job History*   | http://localhost:19888/jobhistory |

While the Hadoop Docker container is running, you can always get the urls' list with the script:

    print-urls.sh

included in the GitHub source repository.


### Available tags:

- Apache Hadoop 3.0.0-cdh6.0.0 ([3.0.0-cdh6.0.0](https://github.com/comchangs/docker-hadoop/blob/3.0.0-cdh6.0.0/Dockerfile))
- Apache Hadoop 2.8.1 ([2.8.1](https://github.com/comchangs/docker-hadoop/blob/2.8.1/Dockerfile))
- Apache Hadoop 2.8.0 ([2.8.0](https://github.com/comchangs/docker-hadoop/blob/2.8.0/Dockerfile))
- Apache Hadoop 2.7.3 ([2.7.3](https://github.com/comchangs/docker-hadoop/blob/2.7.3/Dockerfile))
- Apache Hadoop 2.6.4 ([2.6.4](https://github.com/comchangs/docker-hadoop/blob/2.6.4/Dockerfile))
- Apache Hadoop 2.6.0-cdh5.15.1 ([2.6.0-cdh5.15.1](https://github.com/comchangs/docker-hadoop/blob/2.6.0-cdh5.11.1/Dockerfile))
- Apache Hadoop 2.6.0-cdh5.11.1 ([2.6.0-cdh5.11.1](https://github.com/comchangs/docker-hadoop/blob/2.6.0-cdh5.11.1/Dockerfile))