This is a special livy version to compatible with [XSQL](https://github.com/Qihoo360/XSQL), you need to install xsql jars in your build machine before build this branch.

```
cd XSQL
mvn install -Pxsql -Phive -Phive-thriftserver -Pyarn -DskipTests
```

then you can build livy as normal:

```
mvn clean package -DskipTests -Pspark-2.4
```

you can download `.patch` file from this [link](https://github.com/WeiWenda/incubator-livy/commit/6e04080801263ab349a2b6e6b5825ee88415d1ed.patch).