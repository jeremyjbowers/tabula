## What can you do to help make Tabula better?


1. Bug reports and user interface feedback are always appreciated.
2. Front-end
  * Preview pane: Replace the modal with an always-visible data pane.
3. Back-end
  * Convert ColumnGuesser.java into JRuby or jruby_dump_characters into Java. (This will save significant startup time by not having to start the JVM repeatedly. Or implement Nailgun.)
  * Ability to apply a lasso to all subsequent pages in a document.
  * Modify imgAreaSelect (or replace it with another JS library) to allow multiple selects. (The data should probably be concatenated, then made available for viewing/download/clipboard.)
  * Get rid of XML representation of PDF files.

## How to contribute


1. Fork Tabula
2. Create a topic branch - `git checkout -b my_branch`
3. Push to your branch - `git push origin my_branch`
4. Create a Pull Request from your branch

### Tests

We want to be extra careful about changes in the table extractor [`lib/tabula.rb`](lib/tabula.rb). It is a highly heuristic process and it can regress easily.
If you're doing changes to the table extraction code, please consider adding tests to [`test/test_table_analyze.rb`](test/test_table_analyzer.rb)

