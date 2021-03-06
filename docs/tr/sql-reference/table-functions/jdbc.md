---
machine_translated: true
machine_translated_rev: e8cd92bba3269f47787db090899f7c242adf7818
toc_priority: 43
toc_title: jdbc
---

# jdbc {#table-function-jdbc}

`jdbc(jdbc_connection_uri, schema, table)` - JDBC sürücüsü ile bağlı döner tablo.

Bu tablo işlevi ayrı gerektirir `clickhouse-jdbc-bridge` program çalıştırılacak.
Bu (sorgulanan uzak tablonun DDL dayalı) null türleri destekler.

**Örnekler**

``` sql
SELECT * FROM jdbc('jdbc:mysql://localhost:3306/?user=root&password=root', 'schema', 'table')
```

``` sql
SELECT * FROM jdbc('mysql://localhost:3306/?user=root&password=root', 'schema', 'table')
```

``` sql
SELECT * FROM jdbc('datasource://mysql-local', 'schema', 'table')
```

[Orijinal makale](https://clickhouse.tech/docs/en/query_language/table_functions/jdbc/) <!--hide-->
