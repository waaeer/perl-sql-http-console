# perl-sql-http-console
A demonstration perl SQL HTTP server

## Prerequisites

Based on Mons Andersen's [AnyEvent HTTP-Server-II](https://github.com/Mons/AnyEvent-HTTP-Server-II) and Salvador Fandiño García's [AnyEvent::PgPool](https://metacpan.org/release/AnyEvent-Pg).
Please install them from github and CPAN respectively.

Then run the server:

 perl sql_httpd.pl [ --dbport=5930 ] [ --dbuser=postgres ] [ --port=8019 ] --dbname=ngts2 

Then point your browser to http://localhost:8019/

Note that this server is completely insecure, never use it in production environment.



