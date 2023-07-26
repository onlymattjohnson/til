# Fix No Schema Has Been Selected

The no schema has been selected error occurs because of an empty search path. This can be resolved by connecting to `psql` in the command line and entering

```
> ALTER ROLE username SET search_path = public;
```