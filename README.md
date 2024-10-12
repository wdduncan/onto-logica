# onto-logica
This project uses [logica](https://github.com/EvgSkv/logica) to interacts with ontologies.  

An ontology is loaded in an SQLite database using [rdftab](https://github.com/ontodev/rdftab.rs) and datalog queries are executed against the datase. In many respects, it is similar to the [semantic-sql](https://github.com/INCATools/semantic-sql), but does not require [Soufflé](https://github.com/souffle-lang/souffle).
