# Database connections
Depending on your choice of driver (sync or async) and pooling, your generated queries will accept different types of connections.

The following list details supported connections for each configuration.

## Sync
* `postgres::Client`
* `postgres::Transaction`

## Async
* `tokio_postgres::Client`
* `tokio_postgres::Transaction`

## Async + Deadpool
* `tokio_postgres::Client`
* `tokio_postgres::Transaction`
* `deadpool_postgres::Client`
* `deadpool_postgres::Transaction`

Keep in mind that the Clorinde generated crate re-exports all these modules.
