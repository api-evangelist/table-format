# Table Format (table-format)

Open Table Format is a category of open standards for organizing and managing data in data lakehouses. The three dominant formats are Apache Iceberg (the emerging industry standard with snapshot-based metadata and broad engine support), Delta Lake (Databricks-originated, transaction-log-based), and Apache Hudi (upsert-optimized with Copy-on-Write and Merge-on-Read modes). These formats bring ACID transactions, schema evolution, time travel, and efficient query planning to data lake storage. Apache Iceberg defines a REST Catalog API (OpenAPI spec) that enables standardized catalog operations across implementations like Polaris, Nessie, AWS Glue, and Google BigLake.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Data Lakehouse
- Open Table Format
- Apache Iceberg
- Delta Lake
- Apache Hudi
- Data Lake
- ACID Transactions
- Schema Evolution
- Time Travel

## Timestamps

- **Created:** 2025
- **Modified:** 2026-05-19

## APIs

### Apache Iceberg REST Catalog API

The Apache Iceberg REST Catalog API is an open OpenAPI specification that defines a standard interface for interacting with Apache Iceberg table catalogs. It enables catalog operations including namespace management, table creation, schema updates, and metadata retrieval across any compliant catalog implementation (Polaris, Nessie, AWS Glue, Google BigLake).

- **Human URL:** [https://iceberg.apache.org/rest-catalog-spec/](https://iceberg.apache.org/rest-catalog-spec/)
- **Base URL:** `https://catalog-service/`

#### Tags

- Apache Iceberg
- Data Catalog
- REST Catalog
- Data Lakehouse

#### Properties

- [Documentation](https://iceberg.apache.org/rest-catalog-spec/)
- [OpenAPI](https://github.com/apache/iceberg/blob/main/open-api/rest-catalog-open-api.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Git Hub](https://github.com/apache/iceberg)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/openapi/apache-iceberg-rest-catalog-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/apache-iceberg-rest-catalog.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apache-iceberg-rest-catalog.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Delta Lake

Delta Lake is an open-source storage framework developed by Databricks that adds reliability, performance, and ACID compliance to data lakes. It uses a transaction log (delta log) to record all changes to data. Delta Lake is deeply integrated with Apache Spark and supports batch and streaming workloads, schema enforcement, time travel, and MERGE operations.

- **Human URL:** [https://delta.io/](https://delta.io/)

#### Tags

- Delta Lake
- Data Lake
- ACID Transactions
- Apache Spark
- Databricks

#### Properties

- [Documentation](https://docs.delta.io/)
- [Git Hub](https://github.com/delta-io/delta)
- [Postman Collection](collections/apache-iceberg-rest-catalog.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apache-iceberg-rest-catalog.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apache Hudi

Apache Hudi (Hadoop Upserts Deletes and Incrementals) is an open-source data lakehouse platform optimized for upserts, deletes, and incremental data processing. It supports Copy-on-Write (COW) and Merge-on-Read (MOR) table types and is used for CDC-based data pipelines and streaming analytics.

- **Human URL:** [https://hudi.apache.org/](https://hudi.apache.org/)

#### Tags

- Apache Hudi
- Data Lake
- CDC
- Incremental Processing

#### Properties

- [Documentation](https://hudi.apache.org/docs/overview/)
- [Git Hub](https://github.com/apache/hudi)
- [Postman Collection](collections/apache-iceberg-rest-catalog.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apache-iceberg-rest-catalog.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Unity Catalog

Unity Catalog is an open-source, multi-modal catalog for data and AI that supports Apache Iceberg REST Catalog API, Apache Hive Metastore (HMS) API, and Delta Sharing. It provides unified governance across Delta Lake, Iceberg, and Hudi tables with an OpenAPI specification under Apache 2.0 license.

- **Human URL:** [https://www.unitycatalog.io/](https://www.unitycatalog.io/)

#### Tags

- Data Catalog
- Unity Catalog
- Data Governance
- Multi-format

#### Properties

- [Documentation](https://www.unitycatalog.io/)
- [OpenAPI](https://github.com/unitycatalog/unitycatalog/blob/main/api/all.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Git Hub](https://github.com/unitycatalog/unitycatalog)
- [Postman Collection](collections/apache-iceberg-rest-catalog.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apache-iceberg-rest-catalog.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Wikipedia](https://en.wikipedia.org/wiki/Apache_Iceberg)
- [Apache  Iceberg](https://iceberg.apache.org/)
- [Delta  Lake](https://delta.io/)
- [Apache  Hudi](https://hudi.apache.org/)
- [Unity  Catalog](https://www.unitycatalog.io/)
- [Apache  Iceberg  Git Hub](https://github.com/apache/iceberg)
- [Delta  Lake  Git Hub](https://github.com/delta-io/delta)
- [Apache  Hudi  Git Hub](https://github.com/apache/hudi)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/vocabulary/table-format-vocabulary.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
