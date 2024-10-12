# Data
Directory for storing data to test onto-logic.  


The `prefix.sql` file contains SQL commands to build an SQLite database of common prefixes. It is needed by `rdftab` to build the tables.  
The SQLite database `dental-material.db` contains the tables built by running `rdftab`.  

To build `dental-material.db`, you can execute the following commands:
```
sqlite3 dental-material.db < prefix.sql  
rdftab dental-material.db < dental_material_ontology.owl  
```
For convenience, the shell script `build-dental-materal-db.sh` is provided to execute these commands.
