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

```shell
pip3 install mkdocs-pages-json-plugin
```

Or directly from the git repo

```shell
pip3 install git+https://github.com/userbradley/mkdocs-pages-json-plugin.git
```


```yaml
plugins:
  - pages-json:
        output_file: 'api/pages.json'
```

## Using

You should now be able to go to your site, and the path you chose (for example `api/pages.json`) and see the file.

An example of this in action: https://documentation.breadnet.co.uk/api/pages.json

## What's the point of this?

Eventually I will get around to writing a Mattermost bot or something that will go through the API and send messages when a 
page has expired. 

---

Built by Bradley, with love in the UK. Licensed under MIT so you can do what ever you want with this
