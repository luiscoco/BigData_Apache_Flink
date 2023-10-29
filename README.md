# BigData Apache Flink

https://flink.apache.org/

# What is Apache Flink?

Stateful Computations over Data Streams

Apache Flink is a framework and distributed processing engine for stateful computations over unbounded and bounded data streams

Flink has been designed to run in all common cluster environments, perform computations at in-memory speed and at any scale

# Apache Flink downloads

https://flink.apache.org/downloads/

# Get started with Flink

https://nightlies.apache.org/flink/flink-docs-stable/docs/try-flink/local_installation/

Flink is designed to process continuous streams of data at a lightning fast pace. 

This short guide will show you how to download the latest stable version of Flink, install, and run it. You will also run an example Flink job and view it in the web UI.

## Downloading Flink #
Note: Flink is also available as a Docker image.

Flink runs on all UNIX-like environments, i.e. Linux, Mac OS X, and Cygwin (for Windows). 

You need to have Java 11 installed. 

To check the Java version installed, type in your terminal:

```
java -version
```

Next, download the latest binary release of Flink, then extract the archive:

![image](https://github.com/luiscoco/BigData_Flink/assets/32194879/c4aa3c09-c42e-40ce-ace3-d635676d0313)

![image](https://github.com/luiscoco/BigData_Flink/assets/32194879/cb556c93-b761-4086-a158-ad5827dc7d39)

## Browsing the project directory

Navigate to the extracted directory and list the contents:


For now, you may want to note that:

**bin/** directory contains the flink binary as well as several bash scripts that manage various jobs and tasks

**conf/** directory contains configuration files, including flink-conf.yaml

**examples/** directory contains sample applications that can be used as is with Flink

## Starting and stopping a local cluster #

To **start a local cluster**, run the bash script that comes with Flink:

```
/bin/start-cluster.sh
```

You should see an output like this:

![image](https://github.com/luiscoco/BigData_Flink/assets/32194879/2403bf09-aae5-4558-b9ae-e4d423c572d9)

Flink is now running as a background process. You can check its status with the following command:

```
ps aux | grep flink
```

You should be able to navigate to the web UI at **localhost:8081** to view the Flink dashboard and see that the cluster is up and running.

To quickly **stop the cluster** and all running components, you can use the provided script:

```
/bin/stop-cluster.sh
```


