# yanfs

[![Download](https://api.bintray.com/packages/raisercostin/maven/yanfs/images/download.svg)](https://bintray.com/raisercostin/maven/yanfs/_latestVersion)
[![Build Status](https://travis-ci.org/raisercostin/yanfs.svg?branch=master)](https://travis-ci.org/raisercostin/yanfs)
<!--
[![Codacy Badge](https://www.codacy.com/project/badge/fe1bb28a7735433d89a238ce6f6305c1)](https://www.codacy.com/app/raisercostin/yanfs)
-->

Migrated from https://java.net/projects/yanfs/sources/svn/show

This project represents a Java implementation of the
<a href="http://www.ietf.org/rfc/rfc4506.txt" rel="self">XDR</a>, <a href="http://www.ietf.org/rfc/rfc1831.txt" rel="self">RPC</a>, 
<a href="http://www.ietf.org/rfc/rfc1094.txt"
rel="self">NFSv2</a>, and <a href=
"http://www.ietf.org/rfc/rfc1831.txt"
rel="self">NFSv3</a> protocols in client side form.

WebNFS was the original name for this implementation but the name has changed to reflect the expanded scope of the project to include a server side implementation.

## Maven

### Dependency

```
<dependency>
  <groupId>com.sun</groupId>
  <artifactId>yanfs</artifactId>
  <version>1.4</version>
</dependency>
```

No need to include a repository as is available at https://jcenter.bintray.com/com/sun/yanfs/

# Development
- To release
  `mvn release:prepare release:perform -DskipTests=true -Prelease -Darguments="-DskipTests=true -Prelease"` 
