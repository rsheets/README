# rsheets

**Warning: These projects are in the early scoping stages; do not use for anything other than amusement/frustration purposes**

What is going on here?

* [`rexcel`](https://github.com/rsheets/rexcel)
* [`googlesheets`](https://github.com/jennybc/googlesheets) (update coming soon)

These read spreadsheets into a common intermediate format (see `linen` below).  Rather than reading just the data they read formatting and other metadata, unevaluated formulas, etc.  They can either return a `data.frame` or return a `linen` workbook or worksheet object.

* [`linen`](https://github.com/rsheets/linen) is our general spreadsheet object.

It represents workbooks, worksheets, "views" into worksheets, and formatting information.  It eventually will support a variety of common operations on spreadsheets.

* [`cellranger`](https://github.com/rsheets/cellranger) looks after referencing

Used through out all the other packages, cellranger holds references to regions within worksheets and workbooks.

* [`jailbreakr`](https://github.com/rsheets/jailbreakr) attempts to extract non-tabular data from spreadsheets.

We have collected all the Enron corpus in a [repository on gitlab](https://gitlab.com/rsheets/enron_corpus).  These files can be accessed using [remotefile](https://github.com/richfitz/remotefile), or you can clone the whole ~1.5GB of files.

We ran `rexcel` over all 15871 xlsx files in the corpus and have stored linen objects in [this gitlab repository](https://gitlab.com/rsheets/enron_corpus_linen).  This will be useful (for us) for seeing how Excel is used in the wild.
