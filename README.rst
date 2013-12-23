Sample Session
==============

::

  $ python dbx-keygen-linux.py
  KEYSTORE: unique_id = u'/home/test/.dropbox' 1056782 9088899823225700618
  KEYSTORE: got user key (0, 602a8fceb44dcb5684ac7cd1709625d5)
  User key:  602a8fceb44dcb5684ac7cd1709625d5
  Database key:  d9992bf9748aea34d627174ab2373edb

  $ ~/sqlite3-dbx/sqlite3 -key d9992bf9748aea34d627174ab2373edb .dropbox/config.dbx
  SQLite version 3.7.0
  Enter ".help" for instructions
  Enter SQL statements terminated with a ";"
  sqlite> .tables
  config
  sqlite> select * from config;
  config_schema_version|2
  trace_version|1
  host_id|96d8880c6a4a3d10112f9ba3745ab490
  dropbox_path|/home/test/Dropbox
  ...
