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

    <dependency>
      <groupId>com.sun</groupId>
      <artifactId>yanfs</artifactId>
      <version>1.3</version>
    </dependency>

### Repository
Till the release is added to JCentral you can use this repo

	<repository>
		<id>raisercostin-bintray</id>
		<name>Bintray Raisercostin Maven Repository</name>
		<layout>default</layout>
		<url>https://dl.bintray.com/raisercostin/maven</url>
	</repository>
