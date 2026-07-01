# Changelog

## v1.9.0
**Feature**

- Connection tree: separator rows.
- Connection tree: reorder separators and connections.

**Bug fix**

- PostgreSQL: use of database and schemas. Tree view, structure, data grid, edits, copy-to, and console autocomplete scope to the selected PG schema.

## v1.8.0
**Feature**

- Binary/BLOB cells render as `<binary N bytes>`.
- Page-size options 10 and 20 added.
- `Default Page Size` setting is a dropdown, applied to newly opened grids.
- Read-only connection: F2 value viewer opens the editor read-only.
- Read-only connection: Discard changes reloads the open cell editor to its original value.

**Bug fix**

- CSV/Markdown export: binary cells export as the JSON marker, same as SQL Insert.
- SQL Console export reuses the data-grid exporter and strips binary.
- Copy to connection: generated/computed columns skipped.

## v1.7.1
**Bugs**
- Data grid: text/json value view (F2) for read-only connections
- SQL result: fix column names case

## v1.7.0
**Feature**

- Data grid: checkbox multi-select (per-row plus select-all on the page)
- Data grid: delete selected rows in one transaction (replaces the per-row Delete key / context menu)
- Data grid: copy selected rows into the same-named table on another connection (pick connection + database; strict column check; one transaction)
- SQL Console: Set/Clear SQL Block (right-click) to mark a query block by hand

**Bug fix**

- Export to SQL Insert: correct quotes per engine (backticks for MySQL, double quotes for Postgres)
- Export to SQL Insert: JSON columns export as JSON, not `[object Object]`

## v1.6.0
- Tree: Copy name (right-click, inline icon, Ctrl+C)
- Tree: clicking table keeps tree focus
- Tree: table groups columns/keys/indexes/triggers
- Tree: view and refresh table triggers
- Tree: SQL console files use theme icon
- SQL Console: Multi-DB autocomplete support (cross-database schemas, two-level dotted path completion)

## v1.5.0
- Data-view: per-table filter memory
- Data-view: Recent filters dropdown on WHERE clause
- Extension: Reset filters command

## v1.4.0
- Data-view: show value in tab below
- Read-only connections
- SQL Console improvement, SQL intellisense (autocomplete base SQL functions, keywords)

## v1.3.0
- Built-in SQL formatter with Format CodeLens.

## v1.2.0
- New autocomplete support for alias joins in SQL console.

## v1.1.1
- Expand tables to show columns in tree.
- Expand tables to show indexes in tree.
- Delete key marks rows for deletion.
- Fix arrow navigation in transposed view.
- Consistent DDL view from tree menu.
