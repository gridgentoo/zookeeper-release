код hortonworks : : zookeeper-release-HDP-3.1.4.2-2-tag  
https://github.com/hortonworks/zookeeper-release/tree/HDP-3.1.4.2-2-tag  

Архитектура ZooKeeper  
https://www.youtube.com/playlist?list=PLrTrFnOkIFb3vwhhPF8ShsS8kNsn8emtt  

Профилирование JVM для BigData  
https://www.youtube.com/playlist?list=PLrTrFnOkIFb2Xmx_xuNYsuR0UDGqccJnI  

[_Zookeeper for Enterprise Architect] Архитектура Zookeeper  
https://drive.google.com/drive/folders/1kS1VMu1yWk70R15A4g2jWfECHfnxIpRa  

[Сделать обновление HDP & Ambari & других служб] Аудит установленных пакетов  
https://docs.google.com/document/d/1RxK7codJ4Uvbzn10AJK_GyT1rCPtMTjoQzH3JUxj55s/  

[Инфогра́фика сравнение Версий HDP] что нового в HDP 3.1 архитектуре (и какие версии Сервисы HDP обновлены)  
https://docs.google.com/document/d/1_wrgl8VhExWK8fKmr6Jxv6YEPhT9jXLxejIL72xDMVw/  

For the latest information about ZooKeeper, please visit our website at:

   http://zookeeper.apache.org/

and our wiki, at:

   https://cwiki.apache.org/confluence/display/ZOOKEEPER

Full documentation for this release can also be found in docs/index.html

---------------------------
Packaging/release artifacts

The release artifact contains the following jar file at the toplevel:

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
The content of the legacy jar and the bin+sources jar are the same.

As of version 3.3.0 bin/sources/javadoc jars contained in dist-maven directory
are deployed to the Apache Maven repository after the release has been accepted
by Apache:
  http://people.apache.org/repo/m2-ibiblio-rsync-repository/
© 2019 GitHub, Inc.
