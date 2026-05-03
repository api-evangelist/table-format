# Table Format

Open Table Format is a category of open standards for organizing and managing data in data lakehouses. The three dominant formats are Apache Iceberg (the emerging industry standard), Delta Lake (Databricks-originated), and Apache Hudi (upsert-optimized). These formats bring ACID transactions, schema evolution, time travel, and efficient query planning to data lake storage. Apache Iceberg defines a REST Catalog API that enables standardized catalog operations across implementations.

## APIs

### Apache Iceberg REST Catalog API

An open REST API specification for interacting with Apache Iceberg table catalogs. Provides standard operations for namespace management, table lifecycle, view management, and metadata operations.

- **Documentation:** [https://iceberg.apache.org/rest-catalog-spec/](https://iceberg.apache.org/rest-catalog-spec/)
- **OpenAPI:** [openapi/apache-iceberg-rest-catalog-openapi.yml](openapi/apache-iceberg-rest-catalog-openapi.yml)
- **GitHub:** [https://github.com/apache/iceberg](https://github.com/apache/iceberg)

### Delta Lake

Open-source storage framework with transaction log for ACID compliance on data lakes.
- **Documentation:** [https://docs.delta.io/](https://docs.delta.io/)
- **GitHub:** [https://github.com/delta-io/delta](https://github.com/delta-io/delta)

### Apache Hudi

Lakehouse platform optimized for record-level upserts and incremental data processing.
- **Documentation:** [https://hudi.apache.org/docs/overview/](https://hudi.apache.org/docs/overview/)
- **GitHub:** [https://github.com/apache/hudi](https://github.com/apache/hudi)

### Unity Catalog

Open, multi-modal catalog supporting Iceberg REST Catalog API, Hive Metastore, and Delta Sharing.
- **Website:** [https://www.unitycatalog.io/](https://www.unitycatalog.io/)
- **GitHub:** [https://github.com/unitycatalog/unitycatalog](https://github.com/unitycatalog/unitycatalog)

## Artifacts

### OpenAPI Specifications

| Spec | Description |
|------|-------------|
| [apache-iceberg-rest-catalog-openapi.yml](openapi/apache-iceberg-rest-catalog-openapi.yml) | Apache Iceberg REST Catalog API - namespaces, tables, views, commits |

### JSON Schema

| Schema | Description |
|--------|-------------|
| [table-format-iceberg-table-schema.json](json-schema/table-format-iceberg-table-schema.json) | Schema for Apache Iceberg table metadata (v2 format) |

### JSON Structure

| Structure | Description |
|-----------|-------------|
| [table-format-iceberg-table-structure.json](json-structure/table-format-iceberg-table-structure.json) | Field documentation for Iceberg table metadata |

### JSON-LD

| Context | Description |
|---------|-------------|
| [table-format-context.jsonld](json-ld/table-format-context.jsonld) | Linked data context for table format entities |

### Examples

| Example | Description |
|---------|-------------|
| [apache-iceberg-list-namespaces-example.json](examples/apache-iceberg-list-namespaces-example.json) | List namespaces in a catalog |
| [apache-iceberg-create-table-example.json](examples/apache-iceberg-create-table-example.json) | Create a new Iceberg table |

### Vocabulary

| File | Description |
|------|-------------|
| [table-format-vocabulary.yml](vocabulary/table-format-vocabulary.yml) | Domain vocabulary for open table format concepts |

## Key Concepts

- **Snapshot** - Immutable point-in-time table state enabling time travel
- **Manifest File** - Avro file tracking data files with column-level statistics
- **Catalog** - Service mapping table names to metadata file locations
- **REST Catalog** - Standardized HTTP API for catalog operations
- **Schema Evolution** - Add/drop/rename columns without rewriting data
- **Partition Evolution** - Change partitioning strategy without rewrites
- **ACID Transactions** - Atomicity, Consistency, Isolation, Durability on object storage

## Tags

- Data Lakehouse
- Open Table Format
- Apache Iceberg
- Delta Lake
- Apache Hudi
- ACID Transactions
- Schema Evolution
- Time Travel
