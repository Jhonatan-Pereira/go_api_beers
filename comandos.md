# Comandos executados
```sh
sqlite3 data/beer.db
sqlite3 data/beer_test.db

go mod init github.com/eminetto/pos-web-go

go get github.com/mattn/go-sqlite3

cd core/beer
go test service_test.go
```

# SQL
```sql
CREATE TABLE beer (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name text NOT NULL,
  type integer NOT NULL,
  style integer not null
);
```