# rsheets

What is going on here?

* [`rexcel`](https://github.com/rsheets/rexcel)
* [`googlesheets`](https://github.com/jennybc/googlesheets) (update coming soon)

These read spreadsheets into a common intermediate format (see `linen` below).  Rather than reading just the data they read formatting and other metadata, unevaluated formulas, etc.  They can either return a `data.frame` or return a `linen` workbook or worksheet object.

* [`linen`](https://github.com/rsheets/linen) is our general spreadsheet object.

It represents workbooks, worksheets, "views" into worksheets, and formatting information.  It eventually will support a variety of common operations on spreadsheets.

* [`cellranger`](https://github.com/rsheets/cellranger) looks after referencing

Used through out all the other packages, cellranger holds references to regions within worksheets and workbooks.

* [`jailbreakr`](https://github.com/rsheets/jailbreakr) attempts to extract non-tabular data from spreadsheets.
