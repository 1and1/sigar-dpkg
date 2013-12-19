sigar-java-jni
==============

sigar dpkg packaging for debian.

Create source packages step by step:

```
git clone https://github.com/hyperic/sigar sigar-1.6.4
cd sigar-1.6.4
git checkout sigar-1.6.4
tar czf ../sigar_1.6.4.orig.tar.gz ../sigar-1.6.42
git clone https://github.com/1and1/sigar-java-jni-dpkg debian
cd ..
dpkg-source -b sigar-1.6.4
```

Now the binary package can be built with dpkg-buildpackage or pbuilder the usual way.
