# onto-logica
This project uses [logica](https://github.com/EvgSkv/logica) to interacts with ontologies. Logica is an open source declarative logic programming language for data manipulation. It transforms datalog queries into SQL queries that are executed against a data source.  

Data source supported include:
* SQLite
* DuckDB
* Pandas dataframes

The project uses `poetry` to manage dependencies. However, a `requirements.txt` file is also provided.

## Test data
Test data is provided using a simple [dental material ontology](./data/dental_material_ontology.owl).  
Two SQLite databases are created using the ontology:
* `data/ental-material.db` built using [rdftab](https://github.com/ontodev/rdftab.rs)
* `data/dental_material_ontology.db` built using [semsql](https://github.com/INCATools/semantic-sql)

Details on how to build the databases are provide in [data/READMe.md](./data/README.md).

## Jupyter Lab
Jupyter can be run in `poetry` environment using the command:
* `poetry run jupyter lab --autoreload` (the `--autoreload` is optional)
