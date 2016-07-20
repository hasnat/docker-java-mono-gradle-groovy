
### hasnat/java-mono-gradle-groovy
Docker container containing java, mono, gradle and groovy

## Getting Started

To build docker
```
docker run -d \
    --name app-1 \
    -e HOME=/app \
    -v /app/source/path/on/host:/app/ \
    -v /config/gradle-init:/root/.gradle/ \
    hasnat/java-mono-gradle-groovy
```

To start or attach
```
docker exec -i -t app-1 /bin/bash
```

### Versions
### java

```
root@f26704d183f5:/# java -version
java version "1.8.0_91"
Java(TM) SE Runtime Environment (build 1.8.0_91-b14)
Java HotSpot(TM) 64-Bit Server VM (build 25.91-b14, mixed mode)
```

### mono
```
root@f26704d183f5:/# mono -V
Mono JIT compiler version 3.2.8 (Debian 3.2.8+dfsg-4ubuntu1.1)
Copyright (C) 2002-2014 Novell, Inc, Xamarin Inc and Contributors. www.mono-project.com
	TLS:           __thread
	SIGSEGV:       altstack
	Notifications: epoll
	Architecture:  amd64
	Disabled:      none
	Misc:          softdebug 
	LLVM:          supported, not enabled.
	GC:            sgen
```

### xbuild
```
root@f26704d183f5:/# xbuild /version
XBuild Engine Version 12.0
Mono, Version 3.2.8.0
Copyright (C) 2005-2013 Various Mono authors
```

### doxygen
```
root@f26704d183f5:/# doxygen -v
1.8.6

```

### gradle
```
root@f26704d183f5:/# gradle -v

------------------------------------------------------------
Gradle 2.7
------------------------------------------------------------

Build time:   2015-09-14 07:26:16 UTC
Build number: none
Revision:     c41505168da69fb0650f4e31c9e01b50ffc97893

Groovy:       2.3.10
Ant:          Apache Ant(TM) version 1.9.3 compiled on December 23 2013
JVM:          1.8.0_91 (Oracle Corporation 25.91-b14)
OS:           Linux 3.13.0-83-generic amd64
```

### groovy
```
root@f26704d183f5:/# groovy -v
Groovy Version: 2.4.5 JVM: 1.8.0_91 Vendor: Oracle Corporation OS: Linux
```

## License

This project is licensed under the MIT License
