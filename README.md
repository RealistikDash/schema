# schema
A repository holding RealistikGDPS' current database schema migrations, alongside a Docker image to auto-update them.

All MySQL schema files are stored in `./migrations/` and should be applied sequentially (follow the timestamp).

## Configuration
This tool uses the standard MySQL environment variables for its configuration.

| Variable | Usage |
| --- | --- |
| `MYSQL_HOST` | The hostname to which the migrator will connect (TCP is forced). |
| `MYSQL_TCP_PORT` | The on which the TCP connection will be established. |
| `MYSQL_USER` | The MySQL user responsible for carrying out the migrations. |
| `MYSQL_PASSWORD` | The authentication password for the user provided above. |
