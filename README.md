# Pages json generator

A terrible plugin for mkdocs to generate a `pages.json` file for sites that have a `reviewdate` field on pages

Makes a json file like

```json
[
  {
    "title": "Aqua Page 1",
    "url": "http://127.0.0.1:8000/security/aqua/aqua-page-1/",
    "review_by": "2022-01-01"
  },
  {
    "title": "Aqua Page 2",
    "url": "http://127.0.0.1:8000/security/aqua/aqua-page-2/",
    "review_by": "2022-01-01"
  },
  {
    "title": "Aqua partnership notes",
    "url": "http://127.0.0.1:8000/security/aqua/partnership-info/",
    "review_by": "2022-01-01"
  }
]
```

## Install

```yaml
plugins:
  - pages-json:
        output_file: 'api/pages.json'
```
