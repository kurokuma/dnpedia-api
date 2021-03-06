# dnpedia-api
DnPedia API wrapper for Python

# Usage
```python
# -*- coding: utf-8 -*-

from dnpedia.dnpedia import DnPediaSearch

dp = DnPediaSearch()
print(dp.search("softbank"))
```

- Search Parameters


| Param      | Required/Option | Default       | Type                                       |
|------------|-----------------|---------------|--------------------------------------------|
|   Keyword  | Required        | -             | -                                          |
| match_type | Option          | contains      | startswith/endswith/contains               |
| days       | Option          | 1             | 1~(integer)                                    |
| mode_type  | Option          | recentlyAdded | recentlyAdded/recentlyDeleted/currentZones |

# Returns Sample
```json
{
	"page": 1,
	"total": 1,
	"records": 6,
	"start": 0,
	"limit": 500,
	"rows": [
		{
			"id": 67005854,
			"name": "softbank-jp",
			"zoneid": "com",
			"length": 11,
			"idn": 0,
			"thedate": "2019-11-25"
		},
		{
			"id": 67259935,
			"name": "realsoftbank",
			"zoneid": "com",
			"length": 12,
			"idn": 0,
			"thedate": "2019-11-26"
		},
		{
			"id": 67269976,
			"name": "softbankcert",
			"zoneid": "com",
			"length": 12,
			"idn": 0,
			"thedate": "2019-11-26"
		},
		{
			"id": 67661679,
			"name": "neomsoftbank",
			"zoneid": "com",
			"length": 12,
			"idn": 0,
			"thedate": "2019-11-28"
		},
		{
			"id": 67685334,
			"name": "softbankneom",
			"zoneid": "com",
			"length": 12,
			"idn": 0,
			"thedate": "2019-11-28"
		},
		{
			"id": 68291924,
			"name": "esoftbank",
			"zoneid": "net",
			"length": 9,
			"idn": 0,
			"thedate": "2019-11-30"
		}
	]
}
```