# Hindenburg 

aka A Zeppelin plus a little Spark

A `debian:jessie` based [Spark](https://spark.apache.org/docs/latest/index.html) and [Zeppelin](http://zeppelin.apache.org) Docker container.

This image is large and unapologetically opinionated. It contains:

- [Spark 2.2.0](http://spark.apache.org/docs/2.2.0) and [Hadoop 2.7.3](http://hadoop.apache.org/docs/r2.7.3)
- [PySpark](http://spark.apache.org/docs/2.2.0/api/python) support with [Python 3.4](https://docs.python.org/3.4), [NumPy](http://www.numpy.org), and [SciPy](https://www.scipy.org/scipylib/index.html).

- A partial list of interpreters out-of-the-box. If your favorite interpreter isn't included, consider looking into [adding it with the api](http://zeppelin.apache.org/docs/0.7.3/manual/dynamicinterpreterload.html).
  - spark
  - shell
  - angular
  - jdbc
  - python
  - hbase


## simple usage

To start Zeppelin download this, and then Unzip it into its own folder.
Then once you have done that,navigate to that folder in Terminal and then type

```
docker build .
docker run --rm -p 8090:8090 Hindenburg-master
```

Alternatively, you can pull this prebuilt image:
```
docker pull dylanmei/zeppelin
docker run --rm -p 8090:8090 dylanmei/zeppelin
```
Zeppelin will be running at `http://localhost:8090`.

______________________________________________________________________________________________________________________________

The Folder ZeppelinNotebooks has all sorts of different sample notebooks for interactive tutorials. I still need to label them all. 

