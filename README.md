# Não testei

# mariadb-replication-01

Foi tirado do site: https://github.com/tankibaj/MariaDB-Replication


Command and Usage
./replica <command>

Command	Description
-S, --start, start	Run MariaDB master and slave containers.
-D, --destroy, destroy	Destroy everything related to replica.
-s, -status, status	Replica status.
-SS, --stop-slave	Stop MariaDB slave container.
-ss, --start-slave	Start MariaDB slave container.
-d, --daemon, daemon	Setup a cron job to check replica health at the one-minute interval.
-DD, --destroy-daemon	Destroy cron job for replica health check.
-t, --test, test	Test replica by inseting data in MariaDB.
-T, --stop-test	Stop test.
-l, --log, log	Replica health staus log.
-h, --help, help	Display help list
The test will create a new PHP docker container and a test database titled 'foobar' into the MariaDB master container. It will keep inserting data into the MariaDB master container until you stop the test.
