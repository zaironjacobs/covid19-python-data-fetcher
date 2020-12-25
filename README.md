COVID-19 Data Fetcher
=================

Fetch and save data of each country to a MongoDB database. 

Source of data: https://github.com/CSSEGISandData/COVID-19

An example of a document:

```javascript
{
	"_id" : ObjectId("5fb4e9917a572a64d671bdb7"),
	"name" : "Netherlands",
	"confirmed" : 464205,
	"deaths" : 8689,
	"active" : 449005,
	"recovered" : 6511,
	"last_updated_by_source_at" : ISODate("2020-11-18T05:50:49Z")
}
```

## Dependencies
- [Python 3](https://www.python.org/downloads/)

## Download
```console
$ git clone https://github.com/zaironjacobs/covid19-data-fetcher-python
```

## Usage

Copy the file .env.example to .env and fill in the environment variables.
A local connection example:
```
DATABASE=covid19
COLLECTION=country
CONNECTION_STRING=mongodb://localhost:27017
```

To use:
```console
$ cd covid19-data-fetcher-python
$ pipenv install
$ pipenv run python run.py
```
