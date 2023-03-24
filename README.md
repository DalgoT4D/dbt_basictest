# dbt_basictest
The dbt repository for testing ddp-ui's prefect integration

Add profiles/sim_warehouse.yml containing

sim_warehouse:
  outputs:
    dev:
      type: <DBTYPE> e.g. postgres
      threads: 1
      host: <HOST>
      port: <PORT> e.g. 5432
      user: <USER>
      pass: <PASSWORD>
      dbname: <DBNAME>
      schema: <SCHEMA> e.g. public
