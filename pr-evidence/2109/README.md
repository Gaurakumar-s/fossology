# Multiple license filters

Screenshot from a focused Chromium test using FOSSology's real Twig controls,
Select2, DataTables and license.js. The AJAX responses contain sample findings;
this is not a screenshot of a full FOSSology installation.

The test covers selecting MIT and Apache-2.0, combining scanner and edited
filters, restoring selections after reload, selecting a histogram license,
clearing filters and reading an existing single-license cookie.

Database behavior is tested separately with the PostgreSQL-backed
UploadTreeProxyTest regression cases in the feature branch.
