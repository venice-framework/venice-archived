A pipeline consisting of:
- 3 kafka brokers
- 1 ksql worker
- 1 kafka-connect worker
- 1 postgres database 

Set the topic name and postgres configs in `.env`. 
WARNING: You will also have to set the database name in `postgres/create_database.sql` until https://github.com/venice-framework/venice/issues/3 is fixed.

You will need to provide your own producer. See [python-producer-test](https://github.com/venice-framework/python-producer-test) and [orders_demo](https://github.com/venice-framework/orders_demo) for examples.
