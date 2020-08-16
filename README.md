##What is this?
This is a repackaging of a version of the snowball-stemmer found at https://snowballstem.org/ so that it's available
on Maven Central.

##Maven
```xml
<dependency>
  <groupId>com.github.albarron</groupId>
  <artifactId>snowball-stemmer</artifactId>
  <version>2.0.0</version>
</dependency>
```

##Gradle
This is the original compilation:
```groovy
compile "com.github.albarron:snowball-stemmer:2.0.0"
```
I used this one instead:
```
 gradle build
```
It produces all jar files.

The resulting jar files are currently NOT pushed to maven central. They can be installed locally running
```
mvn install:install-file -Dfile=snowball-stemmer-2.0.0.jar -DgroupId=com.github.albarron -DartifactId=snowball-stemmer -Dversion=2.0.0 -Dpackaging=jar -DgeneratePom=true
```

Anf the dependency can be added as usual in the maven pom file

##Versioning
In the absence of tags, branches, or releases in the original project SVN repository to call out a version, let's go
with what [PyStemmer](https://pypi.python.org/pypi/PyStemmer) is currently using and tack on the SVN revision number at
the end followed by my patch revision number (to fix anything weird that I ---that means rholder--- introduce). For the initial version, we'll
use 1.3.0.581.1. The current version is 2.0.0

##License
This is a copy of the details about the license from [here](https://snowballstem.org/license.html):

```
Except where explicitly noted, all the software given out on this Snowball site is covered by the 3-clause BSD License:


Copyright (c) 2001, Dr Martin Porter,
Copyright (c) 2002, Richard Boulton.
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

Essentially, all this means is that you can do what you like with the code, except claim another Copyright for it, or claim that it is issued under a different license. The software is also issued without warranties, which means that if anyone suffers through its use, they cannot come back and sue you. You also have to alert anyone to whom you give the Snowball software to the fact that it is covered by the BSD license. 
```

##References
* https://snowballstem.org
* https://github.com/snowballstem
