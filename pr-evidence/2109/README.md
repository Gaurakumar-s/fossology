# Multiple license filters

Screenshot from a focused Chromium test using FOSSology's real Twig controls,
Select2, DataTables and license.js. The AJAX responses contain sample findings;
this is not a screenshot of a full FOSSology installation.

The test covers selecting MIT and Apache-2.0, combining scanner and edited
filters, restoring selections after reload, selecting a histogram license,
clearing filters and reading an existing single-license cookie.

Database behavior is tested separately with the PostgreSQL-backed
UploadTreeProxyTest regression cases in the feature branch.

## Full application check

The live screenshots use FOSSology Docker build 4.7.1.266 (base f80ca9)
with the feature patch applied. A sample ZIP containing MIT, Apache-2.0,
BSD-3-Clause and unlicensed README fixtures was uploaded and scanned by Nomos.
Local clearing decisions were seeded for the three licensed files.

Chromium verified both filter controls, combined filters, tree/flat navigation,
reload, Clear, and histogram links against the real AJAX handler and database.
All checks passed without JavaScript errors. The two selected licenses return
the MIT and Apache files while excluding the BSD file and README.
