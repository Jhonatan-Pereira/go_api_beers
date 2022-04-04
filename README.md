## Setup
### 1 - Create databases
```sh
sqlite3 data/beer.db
sqlite3 data/beer_test.db
```
### 2 - Create table
```sql
CREATE TABLE beer (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name text NOT NULL,
  type integer NOT NULL,
  style integer not null
);
```

### 3 - Run
```sh
go run web/main.go
```

## Build
```sh
go build -o bin/pos-web-main ./web/main.go

./bin/pos-web-main
```

## Auto Format
```sh
go fmt web/main.go
```