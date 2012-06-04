# extrafontdb

The **extrafontdb** package is meant to be used with the **extrafont** package. The
extrafont package contains the code to install and use fonts, while the extrafontdb
package contains the font database. (When initially installed, this package
is essentially empty, except for some directories; the database itself is
created by the extrafont package).

The code and the database are separated into two packages because each time
that the package containing the database is re-installed, the database gets
deleted. By putting the database in a separate package, it is possible to
update the code package without deleting the database and having to re-import
the fonts.

Re-installing this package will re-initialize the font database, and all
font will need to be re-imported.

See [https://github.com/wch/extrafont](https://github.com/wch/extrafont) for more
information.
