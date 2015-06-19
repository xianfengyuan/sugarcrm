# SugarCRM 6.5.20 for Docker

## Run

    docker run --name sugarcrm_db -e MYSQL_ROOT_PASSWORD=<password> -d mariadb
    docker run --name sugarcrm -d --link scrm_db:mysql -p 80:80 franzabzieher/sugarcrm

Point your browser to http://<docker_host_ip>/ and follow the instructions of the installer. The mysql server is available as `mysql' and the `root' password is as set above.

