! = todo

Version 0.10α
-------------
- added acl to ddlx_identify()
- New ddlx_grants(oid) function
- fix ddlx_script(text) dependants bug
- ! support for ...
- ! compiler for particlar pg version

Version 0.9
-----------
- renamed extension to ddlx
- API rename pg_ddlx -> ddlx (it is enough)
- support for event triggers
- support for foreign data wrappers
- support for foreign servers
- support for foreign user mappings
- support for text search configurations (regconfig)
- support for text search dictionaries (regdictionary)
- support for text search parsers and templates
- support for casts
- support for collations
- support for conversions
- permission fixes for non superusers
- renamed pg_ddlx_get_columns function to ddlx_describe
- improved script formatting
- improved regression tests
- bug fixes for ddlx_drop

Version 0.8
-----------
- API rename pg_ddl -> pg_ddlx (think DDL eXtractor)
- add pg_ddlx_create(oid) and pg_ddlx_drop(oid) functions to API
- pg_ddlx_script() now also includes dependant objects
  and wraps the whole thing in with BEGIN/END
- support for regoper, regoperator
- support for regnamespace (grants are missing!)
- fix pg_ddlx_get_triggers() (TRUNCATE and INSTEAD supported)
- more slight banner changes
- more use of format() function for speed and readability

Version 0.7
-----------
- pg_ddl_oid_info() renamed to pg_ddl_identify() and improved with new types
- pg_ddl_script() now works for oid and text arguments
- pg_ddl_script(oid) also handles constraints, triggers and defaults
- slight banner change
- use of format() function for speed and readability
- added pg_ddl_get_dependants() internal function
- aggregate support (not for ordered yet!)

Version 0.6
-----------
- support for regroles
- support for collations on domains
- support for range types

Version 0.5
-----------
- support for foreign tables
- support for reloptions (alter view set)
- bugfix when printing [] before typmod

Version 0.4
-----------
- initial support for base types
- do not dump owner grants on classes
- use CREATE OR REPLACE in extension
- empty index name bug fix

Version 0.3
-----------
- support for column collations

Version 0.2
-----------
- bug fixes
- added META.json

Version 0.1
-----------
- initial version
