# Resource catalog

`resources.csv` is the editable source of truth. Save as UTF-8 CSV, keeping the header names and order. Quote fields containing commas, double quotes, or line breaks using standard CSV quoting. Spreadsheet applications can handle this when exporting CSV.

- `id`: unique stable resource ID. Keep it when editing a resource; use a new ID when adding one.
- `title`, `description`, `url`: original resource text and external destination. Links must use HTTP or HTTPS; a blank URL is allowed.
- `topics`: original listing categories, separated by semicolons. A resource may appear in multiple topics. New topics become buttons automatically.
- `resource_type`, `open_science`, `llm_use`, `discipline`: original metadata; separate multiple values with semicolons. Filter options update automatically.
- `date_recorded`: original site's **Date Recorded**, normalized to YYYY-MM-DD. Leave blank when unknown. This is not a publication date or archive capture date.
- `date_recorded_original`: verbatim date text retained for provenance, e.g. March 3, 2025.
- `source_urls`: archived listing pages that support the record, separated by semicolons.

The initial migration extracted all 35 nonempty rows from five recovered resource listings into 34 unique resources. The duplicate OpenAI Cookbook row was combined, retaining both topics and source URLs. Twenty entries include dates; 14 do not. No dates were inferred from publication URLs or archive capture timestamps. Original descriptions and classifications are preserved.

Run `quarto render` after editing. A Python 3.10+ pre-render script validates the CSV and generates `_catalog.html`, which a Lua filter inserts into the Resource Hub. A post-render hook adds individual resource entries to Quarto's site search index. Browser JavaScript filters this rendered catalog immediately; there is no server or external table library. A pushed CSV change takes effect after the site rebuilds. The original archive remains unchanged.

Generated HTML must not be edited or committed. Run tests and checks with:

```sh
python3 -m pip install -r requirements-dev.txt
python3 -m pytest
ruff check scripts tests
black --check scripts tests
bandit -r scripts
quarto render
```
