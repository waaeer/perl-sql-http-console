# perl-sql-http-console
A demonstration perl SQL HTTP server

## Prerequisites

Based on Mons Andersen's [AnyEvent HTTP-Server-II](https://github.com/Mons/AnyEvent-HTTP-Server-II) and Salvador Fandiño García's [AnyEvent::PgPool](https://metacpan.org/release/AnyEvent-Pg).
Please install them from github and CPAN respectively.


## Usage

Run the server:
```bash
 perl sql_httpd.pl [ --dbport=5930 ] [ --dbuser=postgres ] [ --port=8019 ] --dbname=ngts2 
```

Point your browser to http://localhost:8019/

## Security

Note that this server is completely insecure, never use it in production environment.

## ToDo

- [ ] Better CSS
- [ ] Column names
- [ ] SQL highlighting
- [ ] Query History
- [ ] Pagination
- [ ] Data ordering
- [ ] Some specific SQL generation (for full text search, trees etc)





