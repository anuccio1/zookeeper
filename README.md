# Apache ZooKeeper
![alt text](https://zookeeper.apache.org/images/zookeeper_small.gif "ZooKeeper")
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fanuccio1%2Fzookeeper.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fanuccio1%2Fzookeeper?ref=badge_shield)

For the latest information about Apache ZooKeeper, please visit our website at:

   http://zookeeper.apache.org/

and our wiki, at:

   https://cwiki.apache.org/confluence/display/ZOOKEEPER

Full documentation for this release can also be found in docs/index.html

---------------------------
Packaging/release artifacts

The release artifact contains the following jar file at the top level:

zookeeper-<version>.jar         - legacy jar file which contains all classes
                                  and source files. Prior to version 3.3.0 this
                                  was the only jar file available. It has the 
                                  benefit of having the source included (for
                                  debugging purposes) however is also larger as
                                  a result

The release artifact contains the following jar files in "dist-maven" directory:

zookeeper-<version>.jar         - bin (binary) jar - contains only class (*.class) files
zookeeper-<version>-sources.jar - contains only src (*.java) files
zookeeper-<version>-javadoc.jar - contains only javadoc files

These bin/src/javadoc jars were added specifically to support Maven/Ivy which have 
the ability to pull these down automatically as part of your build process. 
The contents of the legacy jar and the bin + sources jars are the same.

As of version 3.3.0, the bin, sources and javadoc jars contained in the
dist-maven directory are deployed to the central repository after the release
is voted on and approved by the Apache ZooKeeper PMC:

  https://repo1.maven.org/maven2/org/apache/zookeeper/zookeeper/

# Contributing
We always welcome new contributors to the project! See [How to Contribute](https://cwiki.apache.org/confluence/display/ZOOKEEPER/HowToContribute) for details on how to submit patch through pull request and our contribution workflow.




## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fanuccio1%2Fzookeeper.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fanuccio1%2Fzookeeper?ref=badge_large)