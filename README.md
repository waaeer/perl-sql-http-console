# perl-sql-http-console
A demonstration perl SQL HTTP server

## Prerequisites

Based on Mons Andersen's [AnyEvent HTTP-Server-II](https://github.com/Mons/AnyEvent-HTTP-Server-II) and Salvador Fandiño García's [AnyEvent::PgPool](https://metacpan.org/release/AnyEvent-Pg).
Please install them from github and CPAN respectively.

Also contains a "Lite" version is DBI-based and has no nontrivial prerequisites. 
It contains a single-threaded non-event simple homebrew HTTP server.

Javascript libraries (Jquery and Jsonp) are packed inside.

## Usage

Run the server:
```bash
 perl sql_httpd.pl [ --dbport=5930 ] [ --dbuser=postgres ] [ --port=8019 ] --dbname=postgres 
```
or 
```bash
 perl sql_httpd_lite.pl [ --dbport=5930 ] [ --dbuser=postgres ] [ --port=8020 ] --dbname=postgres 
```

Point your browser to http://localhost:8019/ or to http://localhost:8020/ for light version.

## Security

Note that this server is completely insecure, never use it in production environment.

## ToDo

- [ ] Better CSS
- [ ] Display "Wait state" while loading result. In far future: query tracing
- [ ] Work with queries longer than HTTP timeout
- [x] Column names
- [ ] Explain
- [ ] SQL highlighting
- [ ] Query History
- [ ] Pagination
- [ ] Data ordering
- [ ] Some specific SQL generation (for full text search, database structure, recursive trees etc)
- [ ] Graphical result representation
- [ ] Pretty formatting of results of specific types (done for "numeric")
- [ ] Highliting in text search results
- [ ] Ability to save or link queries
- [ ] Displaying result of non-select statements
- [ ] Ctrl+Enter in textarea






