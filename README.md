# mobilitydb-sqlalchemy-notebooks
Docker project to test and run mobilitydb, mobilitydb-sqlalchemy, movingpandas, geopandas in jupyter-notebooks.

## Run

Clone and run with docker-compose.

```bash
git clone https://github.com/MBennGit/mobilitydb-sqlalchemy-notebooks.git
docker-compose up -d
```

## Sources

### jupyter/docker-stacks
Utilizing [base-notebook](https://github.com/jupyter/docker-stacks/tree/master/base-notebook) from project jupyter.
Adapted to implement dependencies:
  * geopandas (conda)
  * movingpandas (conda)
  * SQLAlchemy (conda)
  * mobilitydb-sqlalchemy (pipy)
  * psycopg2-binary (pipy)


### adonmo/mobilitydb-sqlalchemy
Notebooks based on the [Quickstart](https://github.com/adonmo/mobilitydb-sqlalchemy/blob/master/docs/quickstart.rst) documentation from mobility-sqlalchemy.

