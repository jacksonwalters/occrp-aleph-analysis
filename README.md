# occrp-aleph-analysis

[![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

Analysis of datasets available through [OCCRP Aleph](https://aleph.occrp.org/). Primarily using NLP and network tools in Python.

## aleph client tools

A download tool for aleph datasets is available as a command line tool via PyPi:

[https://pypi.org/project/alephclient/](https://pypi.org/project/alephclient/)

```
pip install alephclient
```

The documentation is available here:

[https://docs.aleph.occrp.org/developers/](https://docs.aleph.occrp.org/developers/)

To download datasets, first export the host URL and your Aleph API key:

```
export ALEPHCLIENT_HOST=https://aleph.occrp.org/
export ALEPHCLIENT_API_KEY=<your-api-key>
```

Identify the foreign ID of the dataset in Aleph (visibile in the bottom right hand corner):

```
-f, --foreign-id TEXT    foreign_id of the collection  [required]
```

Finally, run the command to download datasets to the specified directory:

```
alephclient fetchdir --foreign-id <some-foreign-id> --prefix ~/Downloads
```

## datasets

- Swedish Aircraft Registry
  - geocode locations [done]
  - display on map [done]

- Romania — People wanted by the police
  - merge persons and address dataframe [done]
  - geocode locations [done]
  - display on map [done]

- Greece Media Ownership
  - geocode locations [done]
  - display on map [done]
 
- UK Lords Financial Interests Official Data
  - parallel datasets, i.e. not able to merge
