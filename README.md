# SQL

SQL (Structured Query Language) is the ANSI/ISO standard language for managing and querying relational databases. SQL defines the interface for creating, reading, updating, and deleting data in relational database management systems (RDBMS). Database connectivity standards including ODBC and JDBC expose SQL capabilities as programmatic APIs. Current standard: ISO/IEC 9075:2023 (SQL:2023).

**Standard:** [ISO/IEC 9075:2023](https://www.iso.org/standard/76583.html)
**Wikipedia:** [SQL](https://en.wikipedia.org/wiki/SQL)
**Standards Body:** ISO/IEC JTC 1/SC 32

## APIs

| API | Description |
|---|---|
| [ODBC API](https://learn.microsoft.com/en-us/sql/odbc/reference/odbc-programmer-s-reference) | Open Database Connectivity — standard C-language API for SQL database access (ISO/IEC 9075-3) |
| [JDBC API](https://docs.oracle.com/en/java/javase/21/docs/api/java.sql/java/sql/package-summary.html) | Java Database Connectivity — standard Java API for SQL database access (JSR 221) |

## Artifacts

### JSON Schema

- [sql-query-schema.json](json-schema/sql-query-schema.json) — Schema for SQL query request objects as used by database HTTP APIs
- [sql-result-schema.json](json-schema/sql-result-schema.json) — Schema for SQL query result objects including column metadata and rows

### JSON Structure

- [sql-query-structure.json](json-structure/sql-query-structure.json) — Field documentation for SQL query objects

### JSON-LD

- [sql-context.jsonld](json-ld/sql-context.jsonld) — JSON-LD context for SQL vocabulary aligned with W3C, schema.org, and DCAT

### Examples

- [sql-select-query-example.json](examples/sql-select-query-example.json) — Execute a parameterized SELECT query via database HTTP API

### Vocabulary

- [sql-vocabulary.yml](vocabulary/sql-vocabulary.yml) — SQL domain vocabulary: SELECT/INSERT/UPDATE/DELETE, DDL/DML, transactions, ACID, ODBC, JDBC, SQLSTATE

## Key Concepts

SQL is standardized under ISO/IEC 9075, with major revisions including SQL:1999 (recursive queries, OO), SQL:2003 (XML, sequences), SQL:2011 (temporal tables), SQL:2016 (JSON), SQL:2019 (polymorphic tables), and SQL:2023 (property graph queries).

Database connectivity is provided by:

- **ODBC** — Cross-platform C API for accessing any ODBC-compliant database
- **JDBC** — Java standard API for relational database connectivity
- **ORM Frameworks** — Hibernate, JPA, SQLAlchemy, ActiveRecord abstract SQL for application developers

## Tags

ANSI Standard, Data Management, Database, ISO Standard, Query Language, Relational Database, SQL
