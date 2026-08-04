# SQL

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
