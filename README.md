# SapientBlock Blockchain Use Case Dataset

An open, bilingual research dataset of **333 real-world blockchain use cases across 74 industries**. Every record contains German and English titles, summaries and full Markdown content, together with maturity, project status, evidence level, dated sources and editorial review metadata.

- Canonical database: https://www.sapientblock.com/blockchain-use-case-datenbank
- Interactive dataset: https://huggingface.co/datasets/TooKeen/sapientblock-blockchain-use-cases
- Website: https://www.sapientblock.com
- License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

## Files

| File | Description |
|---|---|
| `use_cases.jsonl` | One complete bilingual use case per line |
| `export-metadata.json` | Export timestamp, record count, license and canonical source |
| `HUGGINGFACE_DATASET_CARD.md` | Detailed schema, methodology and citation guidance |
| `CITATION.cff` | Machine-readable citation metadata for GitHub |
| `.zenodo.json` | Metadata used for Zenodo release archiving |

## Quick start

```python
import json

with open("use_cases.jsonl", encoding="utf-8") as file:
    cases = [json.loads(line) for line in file]

print(len(cases))
print(cases[0]["title_en"])
```

## Updating and versioning

The website is the canonical source. A scheduled GitHub workflow checks the published Hugging Face export daily. When the files change, it commits the new data and creates a dated GitHub release. Once this repository is connected to Zenodo, every release is preserved as a citable dataset version.

## Attribution

You may use, share and adapt the dataset, including commercially, under CC BY 4.0. **Attribution is mandatory.** Use the following notice and link:

> Source: SapientBlock (https://www.sapientblock.com), licensed under CC BY 4.0.

For individual cases, also include the `canonical_url` stored in the record. The required notice is embedded in every record as `required_attribution`.

Third-party pages linked in the citations remain subject to their own terms; this dataset licenses its descriptions and metadata, not the contents of those external pages.
