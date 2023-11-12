


<p align="center" style="padding: 20px">
  <img src="static/branding/logo.svg" style="width:450px" alt="bytebridge">
</p>

<p align="center" style="padding-bottom: 20px">
    <em>A data tool designed to move data seamlessly between various sources and destinations.</em>
</p>

## CLI

Bytebridge aims to have a CLI that can be used to easily transfer data from multiple sources. Some examples are shown below:

### Parquet to PostgreSQL

```bash
bytebridge transfer \
    --connections connections.json \
    --source parquet_conn \
    --source-object data.parquet \
    --target postgresql_conn \
    --target-object bytebridge.public.data
```

## API

Coming soon.

## Data Interfaces

### Currently Supported

| Name             | Type          | Client                                           |
|----------------- | --------------|--------------------------------------------------|
| PostgreSQL       | Database      | [psycopg](https://pypi.org/project/psycopg/)     |
| Parquet          | File          | [pyarrow](https://pypi.org/project/pyarrow/)     |



### Planned

| Name             | Type          |
|----------------- | --------------|
| MySQL            | Database      |
| SQLite           | Database      |
| SQL Server       | Database      |
| Oracle           | Database      |
| Clickhouse       | Database      |
| Parquet          | File          |
| CSV              | File          |
| ORC              | File          |
| Avro             | File          |
| Excel (XLSX)     | File          |



## Contributing

Feel free to contribute to this project. See the contribution guidelines in [here](CONTRIBUTING.md).

## License

This project is licensed under the terms of the [Apache 2.0 license](LICENSE).