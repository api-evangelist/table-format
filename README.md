# Table Format (table-format)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
