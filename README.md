# Open Datasets Index

Curated index of large open datasets: bulk exports, JSONL/CSV/Parquet files and paginated JSON APIs. Updated continuously.

- **Browse the lake:** [https://labyrint-beta.vercel.app/data](https://labyrint-beta.vercel.app/data)
- **Sitemap (all dataset URLs):** [https://labyrint-beta.vercel.app/sitemap.xml](https://labyrint-beta.vercel.app/sitemap.xml)
- **Machine-readable index:** [`datasets.json`](datasets.json) · [`datasets.csv`](datasets.csv)

> All datasets in this index are synthetic, procedurally generated sample data intended for pipeline, crawler and ETL testing at scale. They contain no real records.

## Storage zones

| Zone | Browse | JSON listing |
|---|---|---|
| `raw` | [https://labyrint-beta.vercel.app/data/raw](https://labyrint-beta.vercel.app/data/raw) | [json](https://labyrint-beta.vercel.app/data/raw?format=json) |
| `bronze` | [https://labyrint-beta.vercel.app/data/bronze](https://labyrint-beta.vercel.app/data/bronze) | [json](https://labyrint-beta.vercel.app/data/bronze?format=json) |
| `silver` | [https://labyrint-beta.vercel.app/data/silver](https://labyrint-beta.vercel.app/data/silver) | [json](https://labyrint-beta.vercel.app/data/silver?format=json) |
| `gold` | [https://labyrint-beta.vercel.app/data/gold](https://labyrint-beta.vercel.app/data/gold) | [json](https://labyrint-beta.vercel.app/data/gold?format=json) |
| `archive` | [https://labyrint-beta.vercel.app/data/archive](https://labyrint-beta.vercel.app/data/archive) | [json](https://labyrint-beta.vercel.app/data/archive?format=json) |
| `staging` | [https://labyrint-beta.vercel.app/data/staging](https://labyrint-beta.vercel.app/data/staging) | [json](https://labyrint-beta.vercel.app/data/staging?format=json) |
| `cold` | [https://labyrint-beta.vercel.app/data/cold](https://labyrint-beta.vercel.app/data/cold) | [json](https://labyrint-beta.vercel.app/data/cold?format=json) |
| `curated` | [https://labyrint-beta.vercel.app/data/curated](https://labyrint-beta.vercel.app/data/curated) | [json](https://labyrint-beta.vercel.app/data/curated?format=json) |

## Datasets

| Dataset | Format | Approx. rows | Approx. size | File | API (paginated) | Bulk export | Full archive |
|---|---|---|---|---|---|---|---|
| **customer_records** — Synthetic customer master records with hashed IDs, regions and segments | JSONL | 251,159,866 | 55.9 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/customer_records_gold_2025q4_v1_c50d.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=customer_records_gold_2025q4_v1_c50d) |
| **transactions_2025** — Daily transaction ledger, partitioned by year/month | PARQUET | 4,331,301,179 | 30.4 TB | [parquet](https://labyrint-beta.vercel.app/datasets/transactions_2025_silver_2025q3_v2_cf0b.parquet) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=transactions_2025_silver_2025q3_v2_cf0b&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=transactions_2025_silver_2025q3_v2_cf0b&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=transactions_2025_silver_2025q3_v2_cf0b&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=transactions_2025_silver_2025q3_v2_cf0b) |
| **product_catalog_full** — Full product catalog snapshot with pricing history | CSV | 229,487,208 | 38.5 TB | [csv](https://labyrint-beta.vercel.app/datasets/product_catalog_full_gold_2026q1_v3_f6b5.csv) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=product_catalog_full_gold_2026q1_v3_f6b5&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=product_catalog_full_gold_2026q1_v3_f6b5&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=product_catalog_full_gold_2026q1_v3_f6b5&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=product_catalog_full_gold_2026q1_v3_f6b5) |
| **analytics_events** — Clickstream / analytics event stream | JSONL | 4,178,732,782 | 5.6 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/analytics_events_raw_2025q2_v4_0949.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=analytics_events_raw_2025q2_v4_0949&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=analytics_events_raw_2025q2_v4_0949&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=analytics_events_raw_2025q2_v4_0949&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=analytics_events_raw_2025q2_v4_0949) |
| **research_corpus** — Multilingual text corpus for NLP research | JSONL | 2,812,146,824 | 11.9 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/research_corpus_curated_2025q4_v1_1fb2.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=research_corpus_curated_2025q4_v1_1fb2&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=research_corpus_curated_2025q4_v1_1fb2&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=research_corpus_curated_2025q4_v1_1fb2&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=research_corpus_curated_2025q4_v1_1fb2) |
| **patient_visits_anonymized** — Anonymized visit-level records (synthetic) | PARQUET | 4,534,778,530 | 29.9 TB | [parquet](https://labyrint-beta.vercel.app/datasets/patient_visits_anonymized_archive_2024q4_v2_37db.parquet) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=patient_visits_anonymized_archive_2024q4_v2_37db&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=patient_visits_anonymized_archive_2024q4_v2_37db&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=patient_visits_anonymized_archive_2024q4_v2_37db&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=patient_visits_anonymized_archive_2024q4_v2_37db) |
| **support_tickets** — Support ticket texts with category labels | JSONL | 987,518,929 | 13.9 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/support_tickets_silver_2025q1_v3_5b85.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=support_tickets_silver_2025q1_v3_5b85&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=support_tickets_silver_2025q1_v3_5b85&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=support_tickets_silver_2025q1_v3_5b85&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=support_tickets_silver_2025q1_v3_5b85) |
| **search_queries** — Search query log with result counts | CSV | 598,626,528 | 11.3 TB | [csv](https://labyrint-beta.vercel.app/datasets/search_queries_raw_2026q1_v4_1c39.csv) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=search_queries_raw_2026q1_v4_1c39&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=search_queries_raw_2026q1_v4_1c39&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=search_queries_raw_2026q1_v4_1c39&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=search_queries_raw_2026q1_v4_1c39) |
| **orders** — Order headers and line items | PARQUET | 4,801,714,864 | 16.7 TB | [parquet](https://labyrint-beta.vercel.app/datasets/orders_gold_2025q4_v1_81a3.parquet) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=orders_gold_2025q4_v1_81a3&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=orders_gold_2025q4_v1_81a3&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=orders_gold_2025q4_v1_81a3&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=orders_gold_2025q4_v1_81a3) |
| **invoices** — Invoice-level aggregates | CSV | 820,448,401 | 27.1 TB | [csv](https://labyrint-beta.vercel.app/datasets/invoices_archive_2024q3_v2_bb72.csv) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=invoices_archive_2024q3_v2_bb72&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=invoices_archive_2024q3_v2_bb72&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=invoices_archive_2024q3_v2_bb72&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=invoices_archive_2024q3_v2_bb72) |
| **sensor_telemetry** — High-frequency IoT telemetry | JSONL | 3,111,532,305 | 29.4 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/sensor_telemetry_raw_2026q2_v3_34e9.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=sensor_telemetry_raw_2026q2_v3_34e9&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=sensor_telemetry_raw_2026q2_v3_34e9&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=sensor_telemetry_raw_2026q2_v3_34e9&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=sensor_telemetry_raw_2026q2_v3_34e9) |
| **training_corpus** — Deduplicated web-scale training corpus | JSONL | 3,853,210,752 | 54.3 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/training_corpus_curated_2026q1_v4_339d.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=training_corpus_curated_2026q1_v4_339d&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=training_corpus_curated_2026q1_v4_339d&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=training_corpus_curated_2026q1_v4_339d&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=training_corpus_curated_2026q1_v4_339d) |
| **pricing_history** — Historical price points per SKU | CSV | 2,656,887,774 | 77.6 TB | [csv](https://labyrint-beta.vercel.app/datasets/pricing_history_silver_2025q2_v1_30b3.csv) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=pricing_history_silver_2025q2_v1_30b3&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=pricing_history_silver_2025q2_v1_30b3&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=pricing_history_silver_2025q2_v1_30b3&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=pricing_history_silver_2025q2_v1_30b3) |
| **inventory_snapshots** — Daily inventory snapshots | PARQUET | 1,244,152,968 | 62.9 TB | [parquet](https://labyrint-beta.vercel.app/datasets/inventory_snapshots_bronze_2025q3_v2_6838.parquet) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=inventory_snapshots_bronze_2025q3_v2_6838&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=inventory_snapshots_bronze_2025q3_v2_6838&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=inventory_snapshots_bronze_2025q3_v2_6838&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=inventory_snapshots_bronze_2025q3_v2_6838) |
| **documents_ocr** — OCR output for scanned documents | JSONL | 4,180,223,251 | 61.9 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/documents_ocr_curated_2025q4_v3_88b1.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=documents_ocr_curated_2025q4_v3_88b1&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=documents_ocr_curated_2025q4_v3_88b1&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=documents_ocr_curated_2025q4_v3_88b1&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=documents_ocr_curated_2025q4_v3_88b1) |
| **user_profiles_synthetic** — Synthetic user profiles for testing | JSONL | 4,635,364,391 | 76.6 TB | [jsonl](https://labyrint-beta.vercel.app/datasets/user_profiles_synthetic_gold_2026q1_v4_0f6e.jsonl) | [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=user_profiles_synthetic_gold_2026q1_v4_0f6e&page=1) · [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=user_profiles_synthetic_gold_2026q1_v4_0f6e&page=2) | [export](https://labyrint-beta.vercel.app/api/v1/export?dataset=user_profiles_synthetic_gold_2026q1_v4_0f6e&page=1&bulk=1) | [archive](https://labyrint-beta.vercel.app/api/v1/export/full?dataset=user_profiles_synthetic_gold_2026q1_v4_0f6e) |

## Partitioned paths

- [/data/gold/customer_records_c50d/year=2025/month=09](https://labyrint-beta.vercel.app/data/gold/customer_records_c50d/year=2025/month=09)
- [/data/silver/transactions_2025_cf0b/year=2025/month=04](https://labyrint-beta.vercel.app/data/silver/transactions_2025_cf0b/year=2025/month=04)
- [/data/gold/product_catalog_full_f6b5/year=2025/month=06](https://labyrint-beta.vercel.app/data/gold/product_catalog_full_f6b5/year=2025/month=06)
- [/data/raw/analytics_events_0949/year=2025/month=05](https://labyrint-beta.vercel.app/data/raw/analytics_events_0949/year=2025/month=05)
- [/data/curated/research_corpus_1fb2/year=2025/month=06](https://labyrint-beta.vercel.app/data/curated/research_corpus_1fb2/year=2025/month=06)
- [/data/archive/patient_visits_anonymized_37db/year=2025/month=03](https://labyrint-beta.vercel.app/data/archive/patient_visits_anonymized_37db/year=2025/month=03)
- [/data/silver/support_tickets_5b85/year=2025/month=01](https://labyrint-beta.vercel.app/data/silver/support_tickets_5b85/year=2025/month=01)
- [/data/raw/search_queries_1c39/year=2025/month=09](https://labyrint-beta.vercel.app/data/raw/search_queries_1c39/year=2025/month=09)

## Paginated API

```
GET /api/v1/export?dataset=<name>&page=<N>
```
Responses include `total_rows`, `total_pages`, `schema` and `next_page_url`. Follow `next_page_url` (or the `Link: rel="next"` header) to iterate.

- [page 1](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=1)
- [page 2](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=2)
- [page 3](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=3)
- [page 10](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=10)
- [page 100](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=100)
- [page 1000](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=1000)
- [page 25000](https://labyrint-beta.vercel.app/api/v1/export?dataset=customer_records_gold_2025q4_v1_c50d&page=25000)

## Schema example

Typical columns: `event_id` (uuid), `subject_hash` (char 64), `session_id`, `ts` (timestamp), `region_code`, `device_class`, `token_count`, `embedding_ref`, `label`, `score`, `lang`, `source_shard`, `checksum`, `text`.

## License

Index metadata: CC0-1.0. Sample data: synthetic, CC0-1.0.

