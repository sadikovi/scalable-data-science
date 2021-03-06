Scalable Data Science
=======

Scalable data science is a technical course in the area of Big Data, aimed at the needs of the
emerging data industry in Christchurch and those of certain academic domain experts across
University of Canterbury's Colleges, including, Arts, Science and Engineering. This course uses
Apache Spark, a fast and general engine for large-scale data processing via databricks to compute
with datasets that won't fit in a single computer. The course will introduce Spark’s core concepts
via hands-on coding, including resilient distributed datasets and map-reduce algorithms, DataFrame
and Spark SQL on Catalyst, scalable machine-learning pipelines in MlLib and vertex programs using
the distributed graph processing framework of GraphX. We will solve instances of real-world big data
decision problems from various scientific domains.

This is being prepared by Raazesh Sainudiin and Sivanand Sivaram
with assistance from Paul Brouwers and Dillon George.

See [http://www.math.canterbury.ac.nz/~r.sainudiin/courses/ScalableDataScience/](http://www.math.canterbury.ac.nz/~r.sainudiin/courses/ScalableDataScience/) for the latest content as cloud-uploadable and locally browsable notebooks. The
Gitbook version of this content will lag by a few weeks.

All course participants (enrolled and observing students for Semester 1 of 2016) may be able to do a
course project if their project proposal gets approved by Raazesh Sainudiin, the course coordinator.

## Build
Steps to add newly created notebook in Databricks cloud (as `.scala`) into gitbook (`.md`):

- Export notebook from Databricks cloud onto your local machine. We work with `.scala` notebooks
most of the time, so currently we only support those.
- Run `bin/parse-notebook.sh` to convert `.scala` notebook into `.md` document. Script takes input
and output files/directories, also prints some minimal statistics. E.g.
```shell
$ bin/parse-notebook.sh temp/scala-notebook.scala temp/
```
You can specify directory as output, or file. In case of directory markdown file name will be the
same as `.scala` file.

- Save converted notebook into repository / Gitbook.

## Contribute
Please read [how to contribute](./CONTRIBUTING.md).
